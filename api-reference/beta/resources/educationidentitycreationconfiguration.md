---
title: Тип ресурса Едукатионидентитикреатионконфигуратион
description: Определяет параметры создания удостоверений профиля School Data. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут созданы в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507163"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="b0f99-105">Тип ресурса Едукатионидентитикреатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b0f99-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0f99-106">Определяет параметры создания удостоверений профиля School Data.</span><span class="sxs-lookup"><span data-stu-id="b0f99-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="b0f99-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="b0f99-107">These identities include students and teachers.</span></span> <span data-ttu-id="b0f99-108">На основе этих параметров пользователи будут созданы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="b0f99-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="b0f99-109">**Примечание:** Если вы включили синхронизацию каталогов для синхронизации между локальной службой Active Directory и Azure Active Directory (Azure AD), используйте вместо этого ресурс [едукатионидентитиматчингконфигуратион](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f99-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="b0f99-110">Производный от [едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0f99-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b0f99-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0f99-111">Properties</span></span>

| <span data-ttu-id="b0f99-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0f99-112">Property</span></span> | <span data-ttu-id="b0f99-113">Тип</span><span class="sxs-lookup"><span data-stu-id="b0f99-113">Type</span></span> | <span data-ttu-id="b0f99-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b0f99-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b0f99-115">**Усердомаинс**</span><span class="sxs-lookup"><span data-stu-id="b0f99-115">**userDomains**</span></span> | <span data-ttu-id="b0f99-116">Коллекция [едукатионидентитидомаин](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="b0f99-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="b0f99-117">Задает список доменов для использования по типам пользователей.</span><span class="sxs-lookup"><span data-stu-id="b0f99-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="b0f99-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0f99-118">JSON representation</span></span>
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
