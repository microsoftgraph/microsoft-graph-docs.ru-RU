---
title: Тип ресурса Едукатионидентитисинчронизатионконфигуратион
description: Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных. Производные классы определяют поведение синхронизации удостоверений. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1ffa1bbcd3f96c86818c68d350236086d0975187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501796"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="8290f-105">Тип ресурса Едукатионидентитисинчронизатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8290f-105">educationIdentitySynchronizationConfiguration resource type</span></span>

<span data-ttu-id="8290f-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8290f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8290f-107">Абстрактный базовый класс для всех конфигураций синхронизации удостоверения для учебного профиля данных.</span><span class="sxs-lookup"><span data-stu-id="8290f-107">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="8290f-108">Производные классы определяют поведение синхронизации удостоверений.</span><span class="sxs-lookup"><span data-stu-id="8290f-108">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="8290f-109">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="8290f-109">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="8290f-110">Производные типы</span><span class="sxs-lookup"><span data-stu-id="8290f-110">Derived types</span></span>
| <span data-ttu-id="8290f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8290f-111">Type</span></span> | <span data-ttu-id="8290f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8290f-112">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="8290f-113">**едукатионидентитиматчингконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="8290f-113">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="8290f-114">Используйте этот тип для согласования с существующими учетными записями пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8290f-114">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="8290f-115">**едукатионидентитикреатионконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="8290f-115">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="8290f-116">Используйте этот тип для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8290f-116">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8290f-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8290f-117">JSON representation</span></span>
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

