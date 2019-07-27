---
title: Получение члена
description: Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a9752d37fed21ebadbd0e05cc30831b13f30ef5
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917960"
---
# <a name="get-a-member"></a><span data-ttu-id="b52f7-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="b52f7-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52f7-104">Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.</span><span class="sxs-lookup"><span data-stu-id="b52f7-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="b52f7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b52f7-105">Permissions</span></span>
<span data-ttu-id="b52f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b52f7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b52f7-108">Permission type</span></span>      | <span data-ttu-id="b52f7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b52f7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b52f7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b52f7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b52f7-111">AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b52f7-111">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b52f7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b52f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b52f7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b52f7-113">Not supported.</span></span>    |
|<span data-ttu-id="b52f7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b52f7-114">Application</span></span> | <span data-ttu-id="b52f7-115">AdministrativeUnit. Read. ALL, AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b52f7-115">AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b52f7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b52f7-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b52f7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b52f7-117">Request headers</span></span>
| <span data-ttu-id="b52f7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b52f7-118">Name</span></span>      |<span data-ttu-id="b52f7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b52f7-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b52f7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b52f7-120">Authorization</span></span>  | <span data-ttu-id="b52f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b52f7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b52f7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b52f7-123">Request body</span></span>
<span data-ttu-id="b52f7-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b52f7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b52f7-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="b52f7-125">Response</span></span>

<span data-ttu-id="b52f7-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [User](../resources/user.md) или [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b52f7-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52f7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b52f7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b52f7-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b52f7-128">Request</span></span>
<span data-ttu-id="b52f7-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b52f7-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="b52f7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b52f7-130">Response</span></span>
<span data-ttu-id="b52f7-131">Ниже приведен пример респоне.</span><span class="sxs-lookup"><span data-stu-id="b52f7-131">Here is an example of the respone.</span></span> <span data-ttu-id="b52f7-132">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b52f7-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b52f7-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b52f7-133">All of the properties will be returned from an actual call.</span></span>

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
