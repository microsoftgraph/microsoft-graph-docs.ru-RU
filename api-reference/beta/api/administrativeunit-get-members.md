---
title: Получение члена
description: Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 78f62bb4752822d3b988327466fdf78a09b68b28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991736"
---
# <a name="get-a-member"></a><span data-ttu-id="0a334-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="0a334-103">Get a member</span></span>

<span data-ttu-id="0a334-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a334-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a334-105">Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.</span><span class="sxs-lookup"><span data-stu-id="0a334-105">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a334-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a334-106">Permissions</span></span>
<span data-ttu-id="0a334-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a334-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0a334-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a334-109">Permission type</span></span>      | <span data-ttu-id="0a334-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a334-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a334-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a334-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a334-112">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0a334-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0a334-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a334-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a334-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a334-114">Not supported.</span></span>    |
|<span data-ttu-id="0a334-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a334-115">Application</span></span> | <span data-ttu-id="0a334-116">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0a334-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a334-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a334-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0a334-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a334-118">Request headers</span></span>
| <span data-ttu-id="0a334-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0a334-119">Name</span></span>      |<span data-ttu-id="0a334-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0a334-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a334-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a334-121">Authorization</span></span>  | <span data-ttu-id="0a334-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a334-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a334-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a334-124">Request body</span></span>
<span data-ttu-id="0a334-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a334-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a334-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a334-126">Response</span></span>

<span data-ttu-id="0a334-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [User](../resources/user.md) или [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a334-127">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a334-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0a334-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a334-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a334-129">Request</span></span>
<span data-ttu-id="0a334-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a334-130">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="0a334-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a334-131">Response</span></span>
<span data-ttu-id="0a334-132">Ниже приведен пример респоне.</span><span class="sxs-lookup"><span data-stu-id="0a334-132">Here is an example of the respone.</span></span> <span data-ttu-id="0a334-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0a334-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a334-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a334-134">All of the properties will be returned from an actual call.</span></span>

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


