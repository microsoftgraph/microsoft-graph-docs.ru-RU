---
title: Тип ресурса Рискюсерхисторитем
description: Представляет историю риска для пользователей Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 519e2a7fdb6662496cdb660095ec63ce81b849f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521056"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="69b28-103">Тип ресурса Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="69b28-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="69b28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69b28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="69b28-105">Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69b28-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="69b28-106">Методы</span><span class="sxs-lookup"><span data-stu-id="69b28-106">Methods</span></span>

| <span data-ttu-id="69b28-107">Метод</span><span class="sxs-lookup"><span data-stu-id="69b28-107">Method</span></span>   | <span data-ttu-id="69b28-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69b28-108">Return Type</span></span>|<span data-ttu-id="69b28-109">Описание</span><span class="sxs-lookup"><span data-stu-id="69b28-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69b28-110">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="69b28-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="69b28-111">Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="69b28-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="69b28-112">Получение журнала рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69b28-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="69b28-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="69b28-113">Properties</span></span>

| <span data-ttu-id="69b28-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="69b28-114">Property</span></span>       | <span data-ttu-id="69b28-115">Тип</span><span class="sxs-lookup"><span data-stu-id="69b28-115">Type</span></span>    | <span data-ttu-id="69b28-116">Описание</span><span class="sxs-lookup"><span data-stu-id="69b28-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="69b28-117">userId</span><span class="sxs-lookup"><span data-stu-id="69b28-117">userId</span></span>         | <span data-ttu-id="69b28-118">строка</span><span class="sxs-lookup"><span data-stu-id="69b28-118">string</span></span>  | <span data-ttu-id="69b28-119">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="69b28-119">The id of the user.</span></span> |
| <span data-ttu-id="69b28-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="69b28-120">initiatedBy</span></span>    | <span data-ttu-id="69b28-121">логический</span><span class="sxs-lookup"><span data-stu-id="69b28-121">bool</span></span>    | <span data-ttu-id="69b28-122">Идентификатор субъекта, который выполняет операцию.</span><span class="sxs-lookup"><span data-stu-id="69b28-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="69b28-123">activity</span><span class="sxs-lookup"><span data-stu-id="69b28-123">activity</span></span>       | [<span data-ttu-id="69b28-124">рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="69b28-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="69b28-125">Действие, связанное с изменением уровня риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="69b28-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="69b28-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69b28-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
