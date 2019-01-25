    ---
<span data-ttu-id="83284-101">Заголовок: описание «educationIdentitySynchronizationConfiguration ресурсов типа»: «абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций.</span><span class="sxs-lookup"><span data-stu-id="83284-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="83284-102">Производные классы определите поведение синхронизации удостоверения.</span><span class="sxs-lookup"><span data-stu-id="83284-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="83284-103">Ниже приведены производных типов.»</span><span class="sxs-lookup"><span data-stu-id="83284-103">The following are the derived types."</span></span>
<span data-ttu-id="83284-104">Автор: «mmast-msft» localization_priority: обычный ms.prod: «education»</span><span class="sxs-lookup"><span data-stu-id="83284-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="83284-105">Тип ресурса educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="83284-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83284-106">Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций.</span><span class="sxs-lookup"><span data-stu-id="83284-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="83284-107">Производные классы определите поведение синхронизации удостоверения.</span><span class="sxs-lookup"><span data-stu-id="83284-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="83284-108">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="83284-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="83284-109">Производные типы</span><span class="sxs-lookup"><span data-stu-id="83284-109">Derived types</span></span>
| <span data-ttu-id="83284-110">Тип</span><span class="sxs-lookup"><span data-stu-id="83284-110">Type</span></span> | <span data-ttu-id="83284-111">Описание</span><span class="sxs-lookup"><span data-stu-id="83284-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="83284-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="83284-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="83284-113">Этот тип используется в соответствии с существующим учетным записям пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="83284-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="83284-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="83284-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="83284-115">Этот тип используется для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="83284-115">Use this type to create new user accounts in Azure AD.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
