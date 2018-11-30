---
title: Получение administrativeUnit
description: Получение простого каталог **administrativeUnit** , соответствующий этой **educationSchool**.
ms.openlocfilehash: 49ac05b44bc89f827091c3b846885a58cb7b8956
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079000"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="c6c07-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c6c07-103">Get administrativeUnit</span></span>

> <span data-ttu-id="c6c07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6c07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6c07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6c07-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6c07-106">Получение простого каталог **administrativeUnit** , соответствующий этой **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="c6c07-106">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="c6c07-107">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="c6c07-107">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="c6c07-108">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="c6c07-108">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6c07-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6c07-109">Permissions</span></span>
<span data-ttu-id="c6c07-110">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="c6c07-110">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="c6c07-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6c07-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6c07-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6c07-112">Permission type</span></span>      | <span data-ttu-id="c6c07-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6c07-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6c07-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6c07-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c6c07-115">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6c07-115">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="c6c07-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6c07-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6c07-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6c07-117">Not supported.</span></span>  |
|<span data-ttu-id="c6c07-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6c07-118">Application</span></span> | <span data-ttu-id="c6c07-119">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6c07-119">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="c6c07-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6c07-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="c6c07-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6c07-121">Request headers</span></span>
| <span data-ttu-id="c6c07-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6c07-122">Header</span></span>       | <span data-ttu-id="c6c07-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c6c07-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6c07-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6c07-124">Authorization</span></span>  | <span data-ttu-id="c6c07-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6c07-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6c07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6c07-127">Request body</span></span>
<span data-ttu-id="c6c07-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6c07-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c6c07-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6c07-129">Response</span></span>
<span data-ttu-id="c6c07-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [administrativeUnit](../resources/administrativeunit.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c6c07-130">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6c07-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c6c07-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6c07-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6c07-132">Request</span></span>
<span data-ttu-id="c6c07-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6c07-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeUnit"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
##### <a name="response"></a><span data-ttu-id="c6c07-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6c07-134">Response</span></span>
<span data-ttu-id="c6c07-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6c07-135">The following is an example of the response.</span></span> 

><span data-ttu-id="c6c07-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6c07-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->