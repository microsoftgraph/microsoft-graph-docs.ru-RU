---
title: Тип ресурса Едукатионидентитикреатионконфигуратион
description: Определяет параметры создания удостоверений профиля School Data. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут созданы в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33f96eab7af8b35720afd5946d83c43db0f20c81
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435049"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="4e406-105">Тип ресурса Едукатионидентитикреатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4e406-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e406-106">Определяет параметры создания удостоверений профиля School Data.</span><span class="sxs-lookup"><span data-stu-id="4e406-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="4e406-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="4e406-107">These identities include students and teachers.</span></span> <span data-ttu-id="4e406-108">На основе этих параметров пользователи будут созданы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="4e406-108">Based on these settings, the users will be created in the directory.</span></span>

> [!WARNING]
> <span data-ttu-id="4e406-109">Если вы включили синхронизацию каталогов для синхронизации между локальной службой Active Directory и Azure Active Directory (Azure AD), используйте вместо этого ресурс [едукатионидентитиматчингконфигуратион](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4e406-109">If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="4e406-110">Производный от [едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4e406-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4e406-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e406-111">Properties</span></span>

| <span data-ttu-id="4e406-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e406-112">Property</span></span>    | <span data-ttu-id="4e406-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4e406-113">Type</span></span>                                                             | <span data-ttu-id="4e406-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4e406-114">Description</span></span>                                    |
| :---------- | :--------------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="4e406-115">усердомаинс</span><span class="sxs-lookup"><span data-stu-id="4e406-115">userDomains</span></span> | <span data-ttu-id="4e406-116">Коллекция [едукатионидентитидомаин](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="4e406-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> | <span data-ttu-id="4e406-117">Задает список доменов для использования по типам пользователей.</span><span class="sxs-lookup"><span data-stu-id="4e406-117">Sets the list of domains to use per user type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e406-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e406-118">JSON representation</span></span>

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
      "@odata.type": "microsoft.graph.educationIdentityDomain"
    }
  ]
}
```
