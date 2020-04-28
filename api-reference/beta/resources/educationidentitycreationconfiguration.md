---
title: Тип ресурса Едукатионидентитикреатионконфигуратион
description: Определяет параметры создания удостоверений профиля School Data. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут созданы в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 09d36a87b8ed1485ce112d40ca8b920290e23997
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006383"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="d3886-105">Тип ресурса Едукатионидентитикреатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d3886-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3886-106">Определяет параметры создания удостоверений профиля School Data.</span><span class="sxs-lookup"><span data-stu-id="d3886-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="d3886-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="d3886-107">These identities include students and teachers.</span></span> <span data-ttu-id="d3886-108">На основе этих параметров пользователи будут созданы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d3886-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="d3886-109">**Примечание:** Если вы включили синхронизацию каталогов для синхронизации между локальной службой Active Directory и Azure Active Directory (Azure AD), используйте вместо этого ресурс [едукатионидентитиматчингконфигуратион](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d3886-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="d3886-110">Производный от [едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3886-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d3886-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3886-111">Properties</span></span>

| <span data-ttu-id="d3886-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3886-112">Property</span></span> | <span data-ttu-id="d3886-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d3886-113">Type</span></span> | <span data-ttu-id="d3886-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d3886-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d3886-115">**усердомаинс**</span><span class="sxs-lookup"><span data-stu-id="d3886-115">**userDomains**</span></span> | <span data-ttu-id="d3886-116">Коллекция [едукатионидентитидомаин](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="d3886-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="d3886-117">Задает список доменов для использования по типам пользователей.</span><span class="sxs-lookup"><span data-stu-id="d3886-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="d3886-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3886-118">JSON representation</span></span>
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
