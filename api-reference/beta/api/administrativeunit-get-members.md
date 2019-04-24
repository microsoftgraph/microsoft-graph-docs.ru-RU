---
title: Получение члена
description: Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 67067d0e465aab61449a42cd833f9e6ce07fcd12
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459633"
---
# <a name="get-a-member"></a><span data-ttu-id="6ed93-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="6ed93-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ed93-104">Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.</span><span class="sxs-lookup"><span data-stu-id="6ed93-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ed93-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ed93-105">Permissions</span></span>
<span data-ttu-id="6ed93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ed93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ed93-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ed93-108">Permission type</span></span>      | <span data-ttu-id="6ed93-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ed93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ed93-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ed93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ed93-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ed93-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ed93-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ed93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ed93-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ed93-113">Not supported.</span></span>    |
|<span data-ttu-id="6ed93-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ed93-114">Application</span></span> | <span data-ttu-id="6ed93-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed93-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ed93-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ed93-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6ed93-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ed93-117">Request headers</span></span>
| <span data-ttu-id="6ed93-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6ed93-118">Name</span></span>      |<span data-ttu-id="6ed93-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6ed93-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ed93-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ed93-120">Authorization</span></span>  | <span data-ttu-id="6ed93-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ed93-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ed93-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ed93-123">Request body</span></span>
<span data-ttu-id="6ed93-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ed93-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ed93-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ed93-125">Response</span></span>

<span data-ttu-id="6ed93-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [User](../resources/user.md) или [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ed93-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ed93-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6ed93-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ed93-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ed93-128">Request</span></span>
<span data-ttu-id="6ed93-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ed93-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="6ed93-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ed93-130">Response</span></span>
<span data-ttu-id="6ed93-131">Ниже приведен пример респоне.</span><span class="sxs-lookup"><span data-stu-id="6ed93-131">Here is an example of the respone.</span></span> <span data-ttu-id="6ed93-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6ed93-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6ed93-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ed93-133">All of the properties will be returned from an actual call.</span></span>

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
