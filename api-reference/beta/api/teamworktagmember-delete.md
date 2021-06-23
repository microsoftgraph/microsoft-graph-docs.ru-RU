---
title: Удаление командной работыTagMember
description: Удаление объекта teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ab64e7053757fed77a086bbdbde4c408813b1879
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060710"
---
# <a name="delete-teamworktagmember"></a><span data-ttu-id="5573a-103">Удаление командной работыTagMember</span><span class="sxs-lookup"><span data-stu-id="5573a-103">Delete teamworkTagMember</span></span>
<span data-ttu-id="5573a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5573a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5573a-105">Удаление [участника из](../resources/teamworktagmember.md) стандартного тега в команде.</span><span class="sxs-lookup"><span data-stu-id="5573a-105">Delete a [member](../resources/teamworktagmember.md) from a standard tag in the team.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5573a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5573a-106">Permissions</span></span>
<span data-ttu-id="5573a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5573a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5573a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5573a-109">Permission type</span></span>|<span data-ttu-id="5573a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5573a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5573a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5573a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5573a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5573a-112">Not supported.</span></span>|
|<span data-ttu-id="5573a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5573a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5573a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5573a-114">Not supported.</span></span>|
|<span data-ttu-id="5573a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5573a-115">Application</span></span>|<span data-ttu-id="5573a-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5573a-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5573a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5573a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}/members/{teamworkTagMember-Id}
```

## <a name="request-headers"></a><span data-ttu-id="5573a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5573a-118">Request headers</span></span>
|<span data-ttu-id="5573a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5573a-119">Name</span></span>|<span data-ttu-id="5573a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5573a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5573a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5573a-121">Authorization</span></span>|<span data-ttu-id="5573a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5573a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5573a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5573a-124">Request body</span></span>
<span data-ttu-id="5573a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5573a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5573a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5573a-126">Response</span></span>

<span data-ttu-id="5573a-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5573a-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5573a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5573a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5573a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5573a-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_teamworktagmember"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==
```


### <a name="response"></a><span data-ttu-id="5573a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5573a-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
