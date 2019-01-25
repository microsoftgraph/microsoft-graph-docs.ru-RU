---
title: Получение члена
description: Используйте этот интерфейс API для получения определенного члена (пользователя или группы) административное подразделение.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67067d0e465aab61449a42cd833f9e6ce07fcd12
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526797"
---
# <a name="get-a-member"></a><span data-ttu-id="57c47-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="57c47-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57c47-104">Используйте этот интерфейс API для получения определенного члена (пользователя или группы) административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="57c47-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="57c47-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57c47-105">Permissions</span></span>
<span data-ttu-id="57c47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="57c47-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57c47-108">Permission type</span></span>      | <span data-ttu-id="57c47-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57c47-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57c47-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57c47-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57c47-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57c47-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57c47-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57c47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57c47-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57c47-113">Not supported.</span></span>    |
|<span data-ttu-id="57c47-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57c47-114">Application</span></span> | <span data-ttu-id="57c47-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57c47-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57c47-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57c47-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="57c47-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57c47-117">Request headers</span></span>
| <span data-ttu-id="57c47-118">Имя</span><span class="sxs-lookup"><span data-stu-id="57c47-118">Name</span></span>      |<span data-ttu-id="57c47-119">Описание</span><span class="sxs-lookup"><span data-stu-id="57c47-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57c47-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57c47-120">Authorization</span></span>  | <span data-ttu-id="57c47-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57c47-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57c47-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57c47-123">Request body</span></span>
<span data-ttu-id="57c47-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57c47-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57c47-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="57c47-125">Response</span></span>

<span data-ttu-id="57c47-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [пользователя](../resources/user.md) или [группы](../resources/group.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="57c47-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c47-127">Пример</span><span class="sxs-lookup"><span data-stu-id="57c47-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57c47-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="57c47-128">Request</span></span>
<span data-ttu-id="57c47-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57c47-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="57c47-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="57c47-130">Response</span></span>
<span data-ttu-id="57c47-131">Ниже приведен пример respone.</span><span class="sxs-lookup"><span data-stu-id="57c47-131">Here is an example of the respone.</span></span> <span data-ttu-id="57c47-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="57c47-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="57c47-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57c47-133">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
