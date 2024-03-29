---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64720cc5416fab704fc094307ea35bc89e4bab34206460e4f4b9e41686cd439c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = new AccessReviewScheduleDefinition
{
    DisplayName = "Review employee access to LinkedIn",
    DescriptionForAdmins = "Review employee access to LinkedIn",
    Scope = new PrincipalResourceMembershipsScope
    {
        PrincipalScopes = new List<AccessReviewScope>()
        {
            new AccessReviewQueryScope
            {
                Query = "/users",
                QueryType = "MicrosoftGraph"
            }
        },
        ResourceScopes = new List<AccessReviewScope>()
        {
            new AccessReviewQueryScope
            {
                Query = "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
                QueryType = "MicrosoftGraph"
            }
        }
    },
    Reviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "./manager",
            QueryType = "MicrosoftGraph",
            QueryRoot = "decisions"
        }
    },
    BackupReviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
            QueryType = "MicrosoftGraph"
        }
    },
    FallbackReviewers = new List<AccessReviewReviewerScope>()
    {
        new AccessReviewReviewerScope
        {
            Query = "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
            QueryType = "MicrosoftGraph"
        }
    },
    Settings = new AccessReviewScheduleSettings
    {
        MailNotificationsEnabled = true,
        ReminderNotificationsEnabled = true,
        JustificationRequiredOnApproval = true,
        DefaultDecisionEnabled = true,
        DefaultDecision = "Recommendation",
        InstanceDurationInDays = 180,
        AutoApplyDecisionsEnabled = true,
        RecommendationsEnabled = true,
        Recurrence = new PatternedRecurrence
        {
            Pattern = new RecurrencePattern
            {
                Type = RecurrencePatternType.AbsoluteMonthly,
                Interval = 6,
                DayOfMonth = 0
            },
            Range = new RecurrenceRange
            {
                Type = RecurrenceRangeType.Numbered,
                StartDate = new Date(2021,5,5),
                EndDate = new Date(2022,5,5)
            }
        }
    }
};

await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .AddAsync(accessReviewScheduleDefinition);

```