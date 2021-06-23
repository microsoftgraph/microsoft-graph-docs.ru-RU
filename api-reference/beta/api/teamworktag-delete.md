---
title: Удаление командной работы
description: Удаляет объект teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 3e23cd6e55122c81973e634cbc47ddaf88402c2d
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060760"
---
# <a name="delete-teamworktag"></a><span data-ttu-id="33e77-103">Удаление командной работы</span><span class="sxs-lookup"><span data-stu-id="33e77-103">Delete teamworkTag</span></span>
<span data-ttu-id="33e77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33e77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33e77-105">Удаление объекта [тега.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="33e77-105">Delete a [tag](../resources/teamworktag.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="33e77-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33e77-106">Permissions</span></span>
<span data-ttu-id="33e77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33e77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33e77-109">Permission type</span></span>|<span data-ttu-id="33e77-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33e77-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33e77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33e77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="33e77-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e77-112">Not supported.</span></span>|
|<span data-ttu-id="33e77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33e77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33e77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e77-114">Not supported.</span></span>|
|<span data-ttu-id="33e77-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="33e77-115">Application</span></span>|<span data-ttu-id="33e77-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e77-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33e77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33e77-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="33e77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33e77-118">Request headers</span></span>
|<span data-ttu-id="33e77-119">Имя</span><span class="sxs-lookup"><span data-stu-id="33e77-119">Name</span></span>|<span data-ttu-id="33e77-120">Описание</span><span class="sxs-lookup"><span data-stu-id="33e77-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="33e77-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33e77-121">Authorization</span></span>|<span data-ttu-id="33e77-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33e77-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33e77-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33e77-124">Request body</span></span>
<span data-ttu-id="33e77-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33e77-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33e77-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="33e77-126">Response</span></span>

<span data-ttu-id="33e77-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="33e77-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="33e77-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="33e77-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="33e77-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="33e77-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_teamworktag"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
```


### <a name="response"></a><span data-ttu-id="33e77-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="33e77-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

