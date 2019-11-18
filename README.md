# APQP Project Template

An implementation of the AIAG standard 5 Phase Project Template.

#### Built Using:
Aras 12.0

#### Versions Tested:
Aras 12.0 (open release)

> Though built and tested using Aras 12.0, this project should function in older releases of Aras 11.0 and Aras 10.0.

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 12.0 SPx preferred)
2. [APQP-Template.xml file](./Data/APQP-Template.xml)
3. [Deliverable_List.xml file](./Fixes/Deliverable_List.xml)

### Install Steps

1. Open up Nash.aspx or AML Studio.
  * You can access Nash via your Aras url: http://localhost/InnovatorServer/Client/scripts/nash.aspx
2. Login using your Aras instance credentials.
3. Copy the contents of `APQP-Template.xml` into Nash or AML Studio. Click **Submit**.
4. Copy the contents of `Deliverable_List.xml` into Nash or AML Studio. Click **Submit**.

### Admin Steps

5. Log in to Aras as admin.
6. Navigate to **Administration > Variables** in the table of contents (TOC).
7. Search for a Variable named `CorporateTimeZone`. If it does not exist, create one and set the value to a time zone name.
  * Example: Set the value to `Eastern Standard Time` for east coast US locations.
8. Navigate to **Templates > Project Templates** in the table of contents (TOC).
9. Select the APQP Template in the main grid.
10. Right click the APQP template and select **Promote**.
11. In the promotion dialog, double click **Approved**.

>Note: To create projects from the APQP template, you will need to promote the Project Template item to "Approved". Otherwise, the template will not appear as an option in the template dropdown list on the New Project form.

You are now ready to use the APQP Project Template.

## Usage

### Creating an APQP Project

1. Log in to Aras as admin.
2. Navigate to **Portfolio > Projects**.
3. Click the **Add New** button.
4. In the Add Project Plan dialog, select **Yes** for Use Template.
5. In the Project Template dropdown list, select **APQP**.
6. Fill in the Project's name and scheduling fields.
7. Click the green checkmark icon to submit the form and create a project form the APQP template.

The newly created project will now open and you can browse the Project Plan tab to view the activities created by the APQP template.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Original code written by Peter Schroer for Aras Corporation.

Documented by Eli Donahue for Aras Labs. @EliJDonahue

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
