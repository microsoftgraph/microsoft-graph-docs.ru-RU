---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972679"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="ab136-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ab136-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab136-106">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="ab136-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="ab136-107">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ab136-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="ab136-108">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="ab136-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="ab136-109">Производные типы</span><span class="sxs-lookup"><span data-stu-id="ab136-109">Derived types</span></span>
| <span data-ttu-id="ab136-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab136-110">Type</span></span> | <span data-ttu-id="ab136-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab136-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="ab136-112">**Едукатионидентитиматчингконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="ab136-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="ab136-113">Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ab136-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="ab136-114">**Едукатионидентитикреатионконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="ab136-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="ab136-115">Используйте этот тип для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ab136-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab136-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab136-116">JSON representation</span></span>
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

