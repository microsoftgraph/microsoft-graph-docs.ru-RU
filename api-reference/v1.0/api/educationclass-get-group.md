---
title: Получение группы
description: Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.
ms.openlocfilehash: 8d77b2869dbde06b24fadaa1f9a3dbd3d5b6d440
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025738"
---
# <a name="get-group"></a><span data-ttu-id="1237f-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="1237f-103">Get group</span></span>

<span data-ttu-id="1237f-104">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="1237f-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="1237f-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="1237f-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="1237f-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="1237f-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="1237f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1237f-107">Permissions</span></span>
<span data-ttu-id="1237f-108">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="1237f-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="1237f-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1237f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1237f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1237f-110">Permission type</span></span>      | <span data-ttu-id="1237f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1237f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1237f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1237f-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1237f-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1237f-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="1237f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1237f-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1237f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1237f-115">Not supported.</span></span>  |
|<span data-ttu-id="1237f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1237f-116">Application</span></span> | <span data-ttu-id="1237f-117">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1237f-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="1237f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1237f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="1237f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1237f-119">Request headers</span></span>
| <span data-ttu-id="1237f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1237f-120">Header</span></span>       | <span data-ttu-id="1237f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1237f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1237f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1237f-122">Authorization</span></span>  | <span data-ttu-id="1237f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1237f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1237f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1237f-125">Request body</span></span>
<span data-ttu-id="1237f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1237f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1237f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1237f-127">Response</span></span>
<span data-ttu-id="1237f-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1237f-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1237f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1237f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1237f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1237f-130">Request</span></span>
<span data-ttu-id="1237f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1237f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
##### <a name="response"></a><span data-ttu-id="1237f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1237f-132">Response</span></span>
<span data-ttu-id="1237f-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1237f-133">The following is an example of the response.</span></span> 

><span data-ttu-id="1237f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1237f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->