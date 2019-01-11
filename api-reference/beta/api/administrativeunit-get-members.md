---
title: Получение члена
description: Используйте этот интерфейс API для получения определенного члена (пользователя или группы) административное подразделение.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 33bbb0a34ba44102c34573059da2efa8824286ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854868"
---
# <a name="get-a-member"></a><span data-ttu-id="552a2-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="552a2-103">Get a member</span></span>

> <span data-ttu-id="552a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="552a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="552a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="552a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="552a2-106">Используйте этот интерфейс API для получения определенного члена (пользователя или группы) административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="552a2-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="552a2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="552a2-107">Permissions</span></span>
<span data-ttu-id="552a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="552a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="552a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="552a2-110">Permission type</span></span>      | <span data-ttu-id="552a2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="552a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="552a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="552a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="552a2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="552a2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="552a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="552a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="552a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="552a2-115">Not supported.</span></span>    |
|<span data-ttu-id="552a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="552a2-116">Application</span></span> | <span data-ttu-id="552a2-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552a2-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="552a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="552a2-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="552a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="552a2-119">Request headers</span></span>
| <span data-ttu-id="552a2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="552a2-120">Name</span></span>      |<span data-ttu-id="552a2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="552a2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="552a2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="552a2-122">Authorization</span></span>  | <span data-ttu-id="552a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="552a2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="552a2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="552a2-125">Request body</span></span>
<span data-ttu-id="552a2-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="552a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="552a2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="552a2-127">Response</span></span>

<span data-ttu-id="552a2-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [пользователя](../resources/user.md) или [группы](../resources/group.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="552a2-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="552a2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="552a2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="552a2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="552a2-130">Request</span></span>
<span data-ttu-id="552a2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="552a2-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="552a2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="552a2-132">Response</span></span>
<span data-ttu-id="552a2-133">Ниже приведен пример respone.</span><span class="sxs-lookup"><span data-stu-id="552a2-133">Here is an example of the respone.</span></span> <span data-ttu-id="552a2-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="552a2-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="552a2-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="552a2-135">All of the properties will be returned from an actual call.</span></span>

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
