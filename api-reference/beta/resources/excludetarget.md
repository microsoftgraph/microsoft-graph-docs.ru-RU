---
title: excludeTarget resource type
description: Представляет пользователей или группы пользователей, которые исключены из политики.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d2786a6107e524fe00430658542dea374cae275
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682948"
---
# <a name="excludetarget-resource-type"></a><span data-ttu-id="e5e5f-103">excludeTarget resource type</span><span class="sxs-lookup"><span data-stu-id="e5e5f-103">excludeTarget resource type</span></span>

<span data-ttu-id="e5e5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5e5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5e5f-105">Представляет пользователей или группы пользователей, которые исключены из политики.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-105">Represents the users or groups of users that are excluded from a policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e5e5f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5e5f-106">Properties</span></span>
|<span data-ttu-id="e5e5f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5e5f-107">Property</span></span>|<span data-ttu-id="e5e5f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e5e5f-108">Type</span></span>|<span data-ttu-id="e5e5f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e5e5f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e5f-110">id</span><span class="sxs-lookup"><span data-stu-id="e5e5f-110">id</span></span>|<span data-ttu-id="e5e5f-111">String</span><span class="sxs-lookup"><span data-stu-id="e5e5f-111">String</span></span>|<span data-ttu-id="e5e5f-112">Идентификатор объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-112">The object identifier of an Azure AD user or group.</span></span>|
|<span data-ttu-id="e5e5f-113">targetType</span><span class="sxs-lookup"><span data-stu-id="e5e5f-113">targetType</span></span>|<span data-ttu-id="e5e5f-114">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="e5e5f-114">authenticationMethodTargetType</span></span>|<span data-ttu-id="e5e5f-115">Тип целевой цели метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-115">The type of the authentication method target.</span></span> <span data-ttu-id="e5e5f-116">Возможные значения: `user`, `group`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-116">Possible values are: `user`, `group`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5e5f-117">Связи</span><span class="sxs-lookup"><span data-stu-id="e5e5f-117">Relationships</span></span>
<span data-ttu-id="e5e5f-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5e5f-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5e5f-119">JSON representation</span></span>
<span data-ttu-id="e5e5f-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5e5f-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludeTarget",
  "id": "String (identifier)",
  "targetType": "String"
}
```
