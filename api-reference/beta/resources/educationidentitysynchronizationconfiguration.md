---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8e193c798f1f3fbc5d4d1c9d8c7b96eed7d39cf9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095361"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="39bf8-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="39bf8-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="39bf8-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39bf8-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39bf8-107">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="39bf8-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="39bf8-108">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="39bf8-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="39bf8-109">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="39bf8-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="39bf8-110">Производные типы</span><span class="sxs-lookup"><span data-stu-id="39bf8-110">Derived types</span></span>

| <span data-ttu-id="39bf8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="39bf8-111">Type</span></span>                                                                                | <span data-ttu-id="39bf8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="39bf8-112">Description</span></span>                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [<span data-ttu-id="39bf8-113">едукатионидентитиматчингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="39bf8-113">educationIdentityMatchingConfiguration</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="39bf8-114">Используйте этот тип для **согласования с существующими** учетными записями пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="39bf8-114">Use this type to **match existing** user accounts in Azure Active Directory.</span></span> |
| [<span data-ttu-id="39bf8-115">едукатионидентитикреатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="39bf8-115">educationIdentityCreationConfiguration</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="39bf8-116">Используйте этот тип для **создания новых** учетных записей пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="39bf8-116">Use this type to **create new** user accounts in Azure Active Directory.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="39bf8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39bf8-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{}
```


