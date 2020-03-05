---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 2b1a7d2c34ff21c8efd57b358864c4d218630594
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519521"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="e4013-103">Тип ресурса Усеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="e4013-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="e4013-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e4013-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4013-105">Представляет счетчик регистраций и состояние для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e4013-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="e4013-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4013-106">Properties</span></span>

| <span data-ttu-id="e4013-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4013-107">Property</span></span>     | <span data-ttu-id="e4013-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e4013-108">Type</span></span>        | <span data-ttu-id="e4013-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4013-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e4013-110">регистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="e4013-110">registrationCount</span></span> | <span data-ttu-id="e4013-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e4013-111">Int64</span></span> | <span data-ttu-id="e4013-112">Предоставляет счетчик регистраций для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4013-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="e4013-113">регистратионстатус</span><span class="sxs-lookup"><span data-stu-id="e4013-113">registrationStatus</span></span> | <span data-ttu-id="e4013-114">String</span><span class="sxs-lookup"><span data-stu-id="e4013-114">String</span></span> | <span data-ttu-id="e4013-115">Представляет состояние регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="e4013-115">Represents the status of user registration.</span></span> <span data-ttu-id="e4013-116">`registered`Возможные значения: `enabled`,, `capable`и. `mfaRegistered`</span><span class="sxs-lookup"><span data-stu-id="e4013-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4013-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4013-117">JSON representation</span></span>

<span data-ttu-id="e4013-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4013-118">The following is a JSON representation of the resource.</span></span>

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