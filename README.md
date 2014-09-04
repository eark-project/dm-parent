dm-parent
=========

eArk WP6 - reference implementation: common Maven configuration

This defined the common properties for all (Java) `dm-*` projects which include
* Version of Hadoop infrastructure tools (CDH), defined as properties. Versions have
  to match  for tools to work together well. For CDH see
  http://www.cloudera.com/content/cloudera-content/cloudera-docs/CDH5/latest/CDH-Version-and-Packaging-Information/cdhvd_cdh_package_previous.html
* Versions of other libraries. Note that Hadoop comes with many transitive dependencies, e.g. Log4j.
  When adding a library the dependency graph needs to be checked for the wanted dependency and if it is
  there then the same version has to be used. **These versions have to be updated accordingly if the
  CDH version is changed!**

TODOs
-----
* put general configurations for Hadoop and others in `src/main/config/`
