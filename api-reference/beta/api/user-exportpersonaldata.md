---
title: 'пользователь: exportPersonalData'
description: Отправляет запрос операции данные политики, внесенные администратором компании для экспорта данных организации пользователя.
ms.openlocfilehash: aceab65992bde3092676a2bfa144498f07f06095
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081028"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="32ec4-103">пользователь: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="32ec4-103">user: exportPersonalData</span></span>

<span data-ttu-id="32ec4-104">Отправляет запрос операции данные политики, внесенные администратором компании для экспорта данных организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="32ec4-104">Submits a data policy operation request, made by a Company Administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="32ec4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32ec4-105">Permissions</span></span>
<span data-ttu-id="32ec4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32ec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32ec4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32ec4-108">Permission type</span></span>      | <span data-ttu-id="32ec4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32ec4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32ec4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32ec4-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="32ec4-111">User.Export.All</span><span class="sxs-lookup"><span data-stu-id="32ec4-111">User.Export.All</span></span>  |
|<span data-ttu-id="32ec4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32ec4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="32ec4-113">Не применимо</span><span class="sxs-lookup"><span data-stu-id="32ec4-113">Not applicable</span></span>  |
|<span data-ttu-id="32ec4-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="32ec4-114">Application</span></span> | <span data-ttu-id="32ec4-115">User.Export.All</span><span class="sxs-lookup"><span data-stu-id="32ec4-115">User.Export.All</span></span> |

><span data-ttu-id="32ec4-116">Примечание: Экспорт может выполняться только администратором компании при использовании делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="32ec4-116">Note: Export can only be performed by a Company Administrator when using the delegated permission.</span></span>

## <a name="http-request"></a><span data-ttu-id="32ec4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32ec4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="32ec4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32ec4-118">Request headers</span></span>
| <span data-ttu-id="32ec4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="32ec4-119">Name</span></span>       | <span data-ttu-id="32ec4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="32ec4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="32ec4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32ec4-121">Authorization</span></span>  | <span data-ttu-id="32ec4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="32ec4-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="32ec4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32ec4-123">Request body</span></span>
<span data-ttu-id="32ec4-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="32ec4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32ec4-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="32ec4-125">Parameter</span></span>    | <span data-ttu-id="32ec4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="32ec4-126">Type</span></span>   |<span data-ttu-id="32ec4-127">Description</span><span class="sxs-lookup"><span data-stu-id="32ec4-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32ec4-128">storageLocation</span><span class="sxs-lookup"><span data-stu-id="32ec4-128">storageLocation</span></span>|<span data-ttu-id="32ec4-129">String</span><span class="sxs-lookup"><span data-stu-id="32ec4-129">String</span></span>|<span data-ttu-id="32ec4-130">Это URL-адрес подписи (SAS) общий доступ к учетной записи хранилища Azure, для которых следует экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="32ec4-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="32ec4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="32ec4-131">Response</span></span>
<span data-ttu-id="32ec4-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="32ec4-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32ec4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="32ec4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32ec4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="32ec4-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```

##### <a name="response"></a><span data-ttu-id="32ec4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="32ec4-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
