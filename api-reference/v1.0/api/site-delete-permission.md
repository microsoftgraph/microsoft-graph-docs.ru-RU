---
title: Разрешения на удаление
description: Удаление объекта разрешений на сайте.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d38b92b9d49863810e6aff0bf7eed0d93643f13f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162127"
---
# <a name="delete-permission"></a><span data-ttu-id="3ed4f-103">Разрешения на удаление</span><span class="sxs-lookup"><span data-stu-id="3ed4f-103">Delete permission</span></span>
<span data-ttu-id="3ed4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ed4f-105">Удаление объекта [разрешений](../resources/permission.md) на сайте.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-105">Delete a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ed4f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ed4f-106">Permissions</span></span>
<span data-ttu-id="3ed4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ed4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ed4f-109">Permission type</span></span>                        | <span data-ttu-id="3ed4f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ed4f-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="3ed4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ed4f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ed4f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-112">Not supported.</span></span>
|<span data-ttu-id="3ed4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ed4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed4f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-114">Not supported.</span></span>
|<span data-ttu-id="3ed4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ed4f-115">Application</span></span>                            | <span data-ttu-id="3ed4f-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3ed4f-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="3ed4f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ed4f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="3ed4f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ed4f-118">Request headers</span></span>
|<span data-ttu-id="3ed4f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3ed4f-119">Name</span></span>|<span data-ttu-id="3ed4f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3ed4f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3ed4f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ed4f-121">Authorization</span></span>|<span data-ttu-id="3ed4f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ed4f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ed4f-124">Request body</span></span>
<span data-ttu-id="3ed4f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ed4f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ed4f-126">Response</span></span>

<span data-ttu-id="3ed4f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ed4f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ed4f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ed4f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ed4f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_permission"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```


### <a name="response"></a><span data-ttu-id="3ed4f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ed4f-131">Response</span></span>
<span data-ttu-id="3ed4f-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ed4f-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Delete site permission"
} -->
