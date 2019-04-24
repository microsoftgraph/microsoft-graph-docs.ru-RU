    ---
<span data-ttu-id="0663e-101">Title: "Едукатионидентитисинчронизатионконфигуратион типа ресурса" Описание: "абстрактный базовый класс для всех конфигураций синхронизации удостоверений профилей учебных данных.</span><span class="sxs-lookup"><span data-stu-id="0663e-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="0663e-102">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0663e-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="0663e-103">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="0663e-103">The following are the derived types."</span></span>
<span data-ttu-id="0663e-104">author: "ммаст — MSFT" локализатион_приорити: Normal MS. произ: "образование"</span><span class="sxs-lookup"><span data-stu-id="0663e-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="0663e-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0663e-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0663e-106">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="0663e-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="0663e-107">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0663e-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="0663e-108">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="0663e-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="0663e-109">ПроизВодные типы</span><span class="sxs-lookup"><span data-stu-id="0663e-109">Derived types</span></span>
| <span data-ttu-id="0663e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0663e-110">Type</span></span> | <span data-ttu-id="0663e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0663e-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="0663e-112">**Едукатионидентитиматчингконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="0663e-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="0663e-113">Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0663e-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="0663e-114">**Едукатионидентитикреатионконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="0663e-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="0663e-115">Используйте этот тип для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0663e-115">Use this type to create new user accounts in Azure AD.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
