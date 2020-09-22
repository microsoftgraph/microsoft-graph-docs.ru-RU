---
title: Тип ресурса Едукатионидентитикреатионконфигуратион
description: Определяет параметры создания удостоверений профиля School Data. К этим удостоверениям относятся студенты и преподаватели. На основе этих параметров пользователи будут созданы в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f4dc03514e3d62f0dca096b0e669ada9247ff39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095403"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="35549-105">Тип ресурса Едукатионидентитикреатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="35549-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35549-106">Определяет параметры создания удостоверений профиля School Data.</span><span class="sxs-lookup"><span data-stu-id="35549-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="35549-107">К этим удостоверениям относятся студенты и преподаватели.</span><span class="sxs-lookup"><span data-stu-id="35549-107">These identities include students and teachers.</span></span> <span data-ttu-id="35549-108">На основе этих параметров пользователи будут созданы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="35549-108">Based on these settings, the users will be created in the directory.</span></span>

> [!WARNING]
> <span data-ttu-id="35549-109">Если вы включили синхронизацию каталогов для синхронизации между локальной службой Active Directory и Azure Active Directory (Azure AD), используйте вместо этого ресурс [едукатионидентитиматчингконфигуратион](educationidentitymatchingconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="35549-109">If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="35549-110">Производный от [едукатионидентитисинчронизатионконфигуратион](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35549-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35549-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="35549-111">Properties</span></span>

| <span data-ttu-id="35549-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="35549-112">Property</span></span>    | <span data-ttu-id="35549-113">Тип</span><span class="sxs-lookup"><span data-stu-id="35549-113">Type</span></span>                                                             | <span data-ttu-id="35549-114">Описание</span><span class="sxs-lookup"><span data-stu-id="35549-114">Description</span></span>                                    |
| :---------- | :--------------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="35549-115">усердомаинс</span><span class="sxs-lookup"><span data-stu-id="35549-115">userDomains</span></span> | <span data-ttu-id="35549-116">Коллекция [едукатионидентитидомаин](educationidentitydomain.md)</span><span class="sxs-lookup"><span data-stu-id="35549-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> | <span data-ttu-id="35549-117">Задает список доменов для использования по типам пользователей.</span><span class="sxs-lookup"><span data-stu-id="35549-117">Sets the list of domains to use per user type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35549-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35549-118">JSON representation</span></span>

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


