---
title: Получение dataPolicyOperation
description: Извлечение свойств объекта dataPolicyOperation.
ms.openlocfilehash: fbc94719f9944adb25f7dd744cf0b15b179f3a5d
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156021"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="09d89-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="09d89-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="09d89-104">Извлечение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="09d89-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09d89-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09d89-105">Permissions</span></span>
<span data-ttu-id="09d89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09d89-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09d89-108">Permission type</span></span>      | <span data-ttu-id="09d89-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09d89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09d89-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09d89-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="09d89-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09d89-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="09d89-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09d89-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="09d89-113">Не применимо</span><span class="sxs-lookup"><span data-stu-id="09d89-113">Not applicable</span></span>  |
|<span data-ttu-id="09d89-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09d89-114">Application</span></span> | <span data-ttu-id="09d89-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09d89-115">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="09d89-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09d89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="09d89-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09d89-117">Request headers</span></span>
| <span data-ttu-id="09d89-118">Имя</span><span class="sxs-lookup"><span data-stu-id="09d89-118">Name</span></span>      |<span data-ttu-id="09d89-119">Описание</span><span class="sxs-lookup"><span data-stu-id="09d89-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09d89-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="09d89-120">Authorization</span></span>  | <span data-ttu-id="09d89-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="09d89-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="09d89-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="09d89-122">Request body</span></span>
<span data-ttu-id="09d89-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09d89-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="09d89-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="09d89-124">Response</span></span>
<span data-ttu-id="09d89-125">Успешно завершена, этот метод возвращает `200 OK` объект [dataPolicyOperation](../resources/datapolicyoperation.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="09d89-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09d89-126">Пример</span><span class="sxs-lookup"><span data-stu-id="09d89-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09d89-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="09d89-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="09d89-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="09d89-128">Response</span></span>
<span data-ttu-id="09d89-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09d89-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value",
  "progress": "progress-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
