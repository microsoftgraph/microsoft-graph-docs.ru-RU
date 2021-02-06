---
title: Тип ресурса userRegistrationCount
description: Представляет количество регистраций и состояние пользователей в клиенте.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5cdcdb4cfd56c0828cfeb7e71defe4c7459e3133
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132953"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="77389-103">Тип ресурса userRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="77389-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="77389-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77389-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77389-105">Представляет количество регистраций и состояние пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="77389-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="77389-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="77389-106">Properties</span></span>

| <span data-ttu-id="77389-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="77389-107">Property</span></span>     | <span data-ttu-id="77389-108">Тип</span><span class="sxs-lookup"><span data-stu-id="77389-108">Type</span></span>        | <span data-ttu-id="77389-109">Описание</span><span class="sxs-lookup"><span data-stu-id="77389-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="77389-110">registrationCount</span><span class="sxs-lookup"><span data-stu-id="77389-110">registrationCount</span></span> | <span data-ttu-id="77389-111">Int64</span><span class="sxs-lookup"><span data-stu-id="77389-111">Int64</span></span> | <span data-ttu-id="77389-112">Предоставляет количество регистраций для вашего клиента.</span><span class="sxs-lookup"><span data-stu-id="77389-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="77389-113">registrationStatus</span><span class="sxs-lookup"><span data-stu-id="77389-113">registrationStatus</span></span> | <span data-ttu-id="77389-114">Строка</span><span class="sxs-lookup"><span data-stu-id="77389-114">String</span></span> | <span data-ttu-id="77389-115">Представляет состояние регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="77389-115">Represents the status of user registration.</span></span> <span data-ttu-id="77389-116">Возможные значения: `registered` , , , и `enabled` `capable` `mfaRegistered` .</span><span class="sxs-lookup"><span data-stu-id="77389-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77389-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="77389-117">JSON representation</span></span>

<span data-ttu-id="77389-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77389-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

