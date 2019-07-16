---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 713bb285e739d9182a982f02975a9b9f46761e3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736518"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="ad9bf-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ad9bf-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad9bf-106">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="ad9bf-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="ad9bf-107">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ad9bf-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="ad9bf-108">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="ad9bf-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="ad9bf-109">Производные типы</span><span class="sxs-lookup"><span data-stu-id="ad9bf-109">Derived types</span></span>
| <span data-ttu-id="ad9bf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ad9bf-110">Type</span></span> | <span data-ttu-id="ad9bf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ad9bf-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="ad9bf-112">**Едукатионидентитиматчингконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="ad9bf-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="ad9bf-113">Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ad9bf-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="ad9bf-114">**Едукатионидентитикреатионконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="ad9bf-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="ad9bf-115">Используйте этот тип для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ad9bf-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad9bf-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad9bf-116">JSON representation</span></span>
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

