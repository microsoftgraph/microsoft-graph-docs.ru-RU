---
title: Тип ресурса Рискюсерхисторитем
description: Представляет историю риска для пользователей Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37f38a649aa3721e65b44e64571dafb797259cf6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620838"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="b46ac-103">Тип ресурса Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="b46ac-103">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b46ac-104">Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b46ac-104">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="b46ac-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b46ac-105">Methods</span></span>

| <span data-ttu-id="b46ac-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b46ac-106">Method</span></span>   | <span data-ttu-id="b46ac-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b46ac-107">Return Type</span></span>|<span data-ttu-id="b46ac-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b46ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b46ac-109">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="b46ac-109">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="b46ac-110">Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b46ac-110">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="b46ac-111">Получение журнала рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b46ac-111">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="b46ac-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b46ac-112">Properties</span></span>

| <span data-ttu-id="b46ac-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b46ac-113">Property</span></span>       | <span data-ttu-id="b46ac-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b46ac-114">Type</span></span>    | <span data-ttu-id="b46ac-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b46ac-115">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="b46ac-116">userId</span><span class="sxs-lookup"><span data-stu-id="b46ac-116">userId</span></span>         | <span data-ttu-id="b46ac-117">string</span><span class="sxs-lookup"><span data-stu-id="b46ac-117">string</span></span>  | <span data-ttu-id="b46ac-118">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="b46ac-118">The id of the user.</span></span> |
| <span data-ttu-id="b46ac-119">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="b46ac-119">initiatedBy</span></span>    | <span data-ttu-id="b46ac-120">bool</span><span class="sxs-lookup"><span data-stu-id="b46ac-120">bool</span></span>    | <span data-ttu-id="b46ac-121">Идентификатор субъекта, который выполняет операцию.</span><span class="sxs-lookup"><span data-stu-id="b46ac-121">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="b46ac-122">activity</span><span class="sxs-lookup"><span data-stu-id="b46ac-122">activity</span></span>       | [<span data-ttu-id="b46ac-123">Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="b46ac-123">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="b46ac-124">Действие, связанное с изменением уровня риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="b46ac-124">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="b46ac-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b46ac-125">JSON representation</span></span>

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
