[Sessions](../jacoco-sessions.md)[maven-code-quality-pom](../index.md)
\> [net.swindle.springdemo.serviceimpl](index.source.md) \>
AgencyRecruitmentServiceImpl.java

# AgencyRecruitmentServiceImpl.java

``` source lang-java  
package net.swindle.springdemo.serviceimpl;

import java.util.Random;

import net.swindle.springdemo.service.RecruitmentService;

/**
 * Agency recruitment service.
 *
 * @author swindle
 */
public class AgencyRecruitmentServiceImpl implements RecruitmentService {

  /* (non-Javadoc)
   * @see net.swindle.springdemo.service.RecruitmentService#recruitEmployees(java.lang.String,
   * java.lang.String, int)
   */
  @Override
  public String recruitEmployees(
      String companyName, String departmentName, int numberOfRecruitments) {
    final Random random = new Random();
    return "\n"
        + companyName
        + "'s "
        + departmentName
        + " hired "
        + random.nextInt(numberOfRecruitments)
        + " employees "
        + "using various hiring agencies.";
  }
}
```

Created with [JaCoCo](http://www.jacoco.org/jacoco) 0.7.9.201702052155