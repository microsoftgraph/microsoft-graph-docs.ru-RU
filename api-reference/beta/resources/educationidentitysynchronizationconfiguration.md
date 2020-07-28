---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c3531999065abc22cc0ecb1870b4bd1bb5f45b7
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45435021"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="0a659-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0a659-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="0a659-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a659-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a659-107">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="0a659-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="0a659-108">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0a659-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="0a659-109">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="0a659-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="0a659-110">Производные типы</span><span class="sxs-lookup"><span data-stu-id="0a659-110">Derived types</span></span>

| <span data-ttu-id="0a659-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0a659-111">Type</span></span>                                                                                | <span data-ttu-id="0a659-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0a659-112">Description</span></span>                                                                         |
| :---------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------- |
| [<span data-ttu-id="0a659-113">едукатионидентитиматчингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0a659-113">educationIdentityMatchingConfiguration</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="0a659-114">Используйте этот тип для **согласования с существующими** учетными записями пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a659-114">Use this type to **match existing** user accounts in Azure Active Directory.</span></span> |
| [<span data-ttu-id="0a659-115">едукатионидентитикреатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0a659-115">educationIdentityCreationConfiguration</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="0a659-116">Используйте этот тип для **создания новых** учетных записей пользователей в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a659-116">Use this type to **create new** user accounts in Azure Active Directory.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="0a659-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a659-117">JSON representation</span></span>

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
