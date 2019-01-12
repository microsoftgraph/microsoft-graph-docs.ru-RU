---
title: Тип ресурса educationIdentityCreationConfiguration
description: Задает параметры, при создании школа данных профиля удостоверений. Эти удостоверения включают студентов и преподавателей. На основе этих параметров, пользователи будут создаваться в каталоге.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: cb7d3d101c547f1ced1b16bf857b7a7e953dc91b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912752"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="c6d22-105">Тип ресурса educationIdentityCreationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6d22-105">educationIdentityCreationConfiguration resource type</span></span>

> <span data-ttu-id="c6d22-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6d22-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6d22-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6d22-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6d22-108">Задает параметры, при создании школа данных профиля удостоверений.</span><span class="sxs-lookup"><span data-stu-id="c6d22-108">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="c6d22-109">Эти удостоверения включают студентов и преподавателей.</span><span class="sxs-lookup"><span data-stu-id="c6d22-109">These identities include students and teachers.</span></span> <span data-ttu-id="c6d22-110">На основе этих параметров, пользователи будут создаваться в каталоге.</span><span class="sxs-lookup"><span data-stu-id="c6d22-110">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="c6d22-111">**Примечание:** Если у вас есть синхронизации каталогов, включенным для синхронизации между локальной службы каталогов Active Directory и Azure Active Directory (Azure AD), используйте [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c6d22-111">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="c6d22-112">На основе [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6d22-112">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c6d22-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6d22-113">Properties</span></span>

| <span data-ttu-id="c6d22-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6d22-114">Property</span></span> | <span data-ttu-id="c6d22-115">Тип</span><span class="sxs-lookup"><span data-stu-id="c6d22-115">Type</span></span> | <span data-ttu-id="c6d22-116">Описание</span><span class="sxs-lookup"><span data-stu-id="c6d22-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c6d22-117">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="c6d22-117">**userDomains**</span></span> | <span data-ttu-id="c6d22-118">[educationIdentityDomain](educationidentitydomain.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c6d22-118">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="c6d22-119">Задает список доменов для использования каждого типа пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6d22-119">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="c6d22-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6d22-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
