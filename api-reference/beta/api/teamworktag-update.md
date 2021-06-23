---
title: Обновление командной работы
description: Обновление свойств объекта teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: a17fcca078e66251a6532b2d3862352485f3cb2f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060713"
---
# <a name="update-teamworktag"></a><span data-ttu-id="91a94-103">Обновление командной работы</span><span class="sxs-lookup"><span data-stu-id="91a94-103">Update teamworkTag</span></span>
<span data-ttu-id="91a94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91a94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91a94-105">Обновление свойств объекта [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="91a94-105">Update the properties of a [teamworkTag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91a94-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91a94-106">Permissions</span></span>
<span data-ttu-id="91a94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91a94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91a94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91a94-109">Permission type</span></span>|<span data-ttu-id="91a94-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91a94-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91a94-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91a94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91a94-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91a94-112">Not supported.</span></span>|
|<span data-ttu-id="91a94-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91a94-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91a94-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91a94-114">Not supported.</span></span>|
|<span data-ttu-id="91a94-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="91a94-115">Application</span></span>|<span data-ttu-id="91a94-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91a94-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91a94-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91a94-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="91a94-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91a94-118">Request headers</span></span>
|<span data-ttu-id="91a94-119">Имя</span><span class="sxs-lookup"><span data-stu-id="91a94-119">Name</span></span>|<span data-ttu-id="91a94-120">Описание</span><span class="sxs-lookup"><span data-stu-id="91a94-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="91a94-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91a94-121">Authorization</span></span>|<span data-ttu-id="91a94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91a94-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="91a94-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91a94-124">Content-Type</span></span>|<span data-ttu-id="91a94-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91a94-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91a94-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91a94-127">Request body</span></span>
<span data-ttu-id="91a94-128">В теле запроса поставляем представление JSON объекта [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="91a94-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="91a94-129">В следующей таблице показаны свойства, необходимые при обновлении [teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="91a94-129">The following table shows the properties that are required when you update the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="91a94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="91a94-130">Property</span></span>|<span data-ttu-id="91a94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="91a94-131">Type</span></span>|<span data-ttu-id="91a94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="91a94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a94-133">displayName</span><span class="sxs-lookup"><span data-stu-id="91a94-133">displayName</span></span>|<span data-ttu-id="91a94-134">Строка</span><span class="sxs-lookup"><span data-stu-id="91a94-134">String</span></span>|<span data-ttu-id="91a94-135">Имя тега.</span><span class="sxs-lookup"><span data-stu-id="91a94-135">Name of the tag.</span></span> <span data-ttu-id="91a94-136">Значение не может быть более 40 символов.</span><span class="sxs-lookup"><span data-stu-id="91a94-136">The value can not be more than 40 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="91a94-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="91a94-137">Response</span></span>

<span data-ttu-id="91a94-138">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [teamworkTag](../resources/teamworktag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="91a94-138">If successful, this method returns a `200 OK` response code and an updated [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91a94-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="91a94-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91a94-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="91a94-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_teamworktag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
Content-Type: application/json
Content-length: 185

{
  "displayName": "Finance"
}
```


### <a name="response"></a><span data-ttu-id="91a94-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="91a94-141">Response</span></span>
><span data-ttu-id="91a94-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91a94-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Finance",
  "memberCount": 2,
  "tagType": "standard"
}
```
