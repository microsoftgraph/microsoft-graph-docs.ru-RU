    ---
<span data-ttu-id="e46b6-101">Title: "Едукатионидентитисинчронизатионконфигуратион типа ресурса" Описание: "абстрактный базовый класс для всех конфигураций синхронизации удостоверений профилей учебных данных.</span><span class="sxs-lookup"><span data-stu-id="e46b6-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="e46b6-102">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e46b6-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="e46b6-103">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="e46b6-103">The following are the derived types."</span></span>
<span data-ttu-id="e46b6-104">author: "ммаст — MSFT" локализатион_приорити: Normal MS. произ: "образование"</span><span class="sxs-lookup"><span data-stu-id="e46b6-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="e46b6-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e46b6-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e46b6-106">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="e46b6-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="e46b6-107">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e46b6-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="e46b6-108">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="e46b6-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="e46b6-109">ПроизВодные типы</span><span class="sxs-lookup"><span data-stu-id="e46b6-109">Derived types</span></span>
| <span data-ttu-id="e46b6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e46b6-110">Type</span></span> | <span data-ttu-id="e46b6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e46b6-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="e46b6-112">**Едукатионидентитиматчингконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="e46b6-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="e46b6-113">Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e46b6-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="e46b6-114">**Едукатионидентитикреатионконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="e46b6-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="e46b6-115">Используйте этот тип для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e46b6-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e46b6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e46b6-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

