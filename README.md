# ETL_CODE_GEN
ETL Code Gen schema of views to produce ddls for view, table, insert, merge and tasks

This code has been produce as a starting block to automate a data plaftorm. It may need slight adjustments to function in your environemnt or in your desired state.

The flow to run the code is:
1. Run the attached build script to create the views in your environment.
2. Load data in a raw format to snowflake using Fivetran or your prefered ELT tool.
3. Populate the Primary Keys table with your primary keys of the data you landed and their corosponding STG and HIST tables.
4. Select DDLs from the VW_GEN_STG_VIEWS and run them to build.
5. Select DDLs from the VW_GEN_HIST_TABLES and run them to build.
6. Select DDLs from the VW_GEN_HIST_VIEWS and run them to build.
7. Create task batches for each schema (see example in build script).
8. Select DDLs from the VW_GEN_HIST_INSERTS and run them to build.
9. Select DDLs from the VW_GEN_HIST_MERGE and run them to build.
10.Complete your automated data plaform is ready to run!

Any issues or bugs please let me know
Linkedin: https://www.linkedin.com/in/dominic-colyer/

Email: dominiccolyer@gmail.com

Thanks!
