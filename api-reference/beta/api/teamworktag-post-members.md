---
title: Создание командной работыTagMember
description: Создайте новый объект teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 28ae8ae4749e1ecca4f5e370858e88de45d2faf4
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060719"
---
# <a name="create-teamworktagmember"></a><span data-ttu-id="ce66f-103">Создание командной работыTagMember</span><span class="sxs-lookup"><span data-stu-id="ce66f-103">Create teamworkTagMember</span></span>
<span data-ttu-id="ce66f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce66f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce66f-105">Создайте новый [объект teamworkTagMember](../resources/teamworktagmember.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="ce66f-105">Create a new [teamworkTagMember](../resources/teamworktagmember.md) object in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce66f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce66f-106">Permissions</span></span>
<span data-ttu-id="ce66f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce66f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce66f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce66f-109">Permission type</span></span>|<span data-ttu-id="ce66f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce66f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce66f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce66f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce66f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce66f-112">Not supported.</span></span>|
|<span data-ttu-id="ce66f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce66f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce66f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce66f-114">Not supported.</span></span>|
|<span data-ttu-id="ce66f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce66f-115">Application</span></span>|<span data-ttu-id="ce66f-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce66f-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce66f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce66f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="request-headers"></a><span data-ttu-id="ce66f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce66f-118">Request headers</span></span>
|<span data-ttu-id="ce66f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ce66f-119">Name</span></span>|<span data-ttu-id="ce66f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ce66f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce66f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce66f-121">Authorization</span></span>|<span data-ttu-id="ce66f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce66f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce66f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce66f-124">Content-Type</span></span>|<span data-ttu-id="ce66f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce66f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce66f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce66f-127">Request body</span></span>
<span data-ttu-id="ce66f-128">В теле запроса поставляем представление JSON объекта [teamworkTagMember.](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="ce66f-128">In the request body, supply a JSON representation of the [teamworkTagMember](../resources/teamworktagmember.md) object.</span></span>

<span data-ttu-id="ce66f-129">В следующей таблице показаны свойства, необходимые при создании [командной работыTagMember.](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="ce66f-129">The following table shows the properties that are required when you create the [teamworkTagMember](../resources/teamworktagmember.md).</span></span>

|<span data-ttu-id="ce66f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce66f-130">Property</span></span>|<span data-ttu-id="ce66f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ce66f-131">Type</span></span>|<span data-ttu-id="ce66f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ce66f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce66f-133">userId</span><span class="sxs-lookup"><span data-stu-id="ce66f-133">userId</span></span>|<span data-ttu-id="ce66f-134">String</span><span class="sxs-lookup"><span data-stu-id="ce66f-134">String</span></span>|<span data-ttu-id="ce66f-135">Идентификатор пользователя члена группы.</span><span class="sxs-lookup"><span data-stu-id="ce66f-135">User identifier of the member of the team.</span></span>|



## <a name="response"></a><span data-ttu-id="ce66f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce66f-136">Response</span></span>

<span data-ttu-id="ce66f-137">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект teamworkTagMember](../resources/teamworktagmember.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce66f-137">If successful, this method returns a `201 Created` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce66f-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ce66f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce66f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce66f-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_teamworktagmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
Content-Type: application/json
Content-length: 144

{
    "userId":"97f62344-57dc-409c-88ad-c4af14158ff5"
}
```


### <a name="response"></a><span data-ttu-id="ce66f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce66f-140">Response</span></span>
><span data-ttu-id="ce66f-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce66f-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Megan Bowen",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
}
```

