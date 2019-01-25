---
title: Тип ресурса educationIdentityCreationConfiguration
description: Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511403"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="862df-105">Тип ресурса educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="862df-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="862df-106">Задает параметры, при создании школа данных профиля удостоверений.</span><span class="sxs-lookup"><span data-stu-id="862df-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="862df-107">Эти удостоверения включают студентов и преподавателей.</span><span class="sxs-lookup"><span data-stu-id="862df-107">These identities include students and teachers.</span></span> <span data-ttu-id="862df-108">На основе этих параметров, пользователи будут создаваться в каталоге.</span><span class="sxs-lookup"><span data-stu-id="862df-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="862df-109">**Примечание:** Если у вас есть синхронизации каталогов, включенным для синхронизации между локальной службы каталогов Active Directory и Azure Active Directory (Azure AD), используйте [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="862df-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="862df-110">На основе [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="862df-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="862df-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="862df-111">Properties</span></span>

| <span data-ttu-id="862df-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="862df-112">Property</span></span> | <span data-ttu-id="862df-113">Тип</span><span class="sxs-lookup"><span data-stu-id="862df-113">Type</span></span> | <span data-ttu-id="862df-114">Описание</span><span class="sxs-lookup"><span data-stu-id="862df-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="862df-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="862df-115">**userDomains**</span></span> | <span data-ttu-id="862df-116">[educationIdentityDomain](educationidentitydomain.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="862df-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="862df-117">Задает список доменов для использования каждого типа пользователя.</span><span class="sxs-lookup"><span data-stu-id="862df-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="862df-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="862df-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
