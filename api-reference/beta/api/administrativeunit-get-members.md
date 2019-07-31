---
title: Получение члена
description: Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81a1165148dbaa81740cdc4d7b9dbf65f7d8cd4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945860"
---
# <a name="get-a-member"></a><span data-ttu-id="eeb65-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="eeb65-103">Get a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeb65-104">Используйте этот API для получения определенного элемента (пользователя или группы) в административной единице.</span><span class="sxs-lookup"><span data-stu-id="eeb65-104">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="eeb65-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb65-105">Permissions</span></span>
<span data-ttu-id="eeb65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eeb65-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eeb65-108">Permission type</span></span>      | <span data-ttu-id="eeb65-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eeb65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeb65-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eeb65-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eeb65-111">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="eeb65-111">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eeb65-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eeb65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeb65-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eeb65-113">Not supported.</span></span>    |
|<span data-ttu-id="eeb65-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eeb65-114">Application</span></span> | <span data-ttu-id="eeb65-115">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="eeb65-115">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeb65-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eeb65-116">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eeb65-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eeb65-117">Request headers</span></span>
| <span data-ttu-id="eeb65-118">Имя</span><span class="sxs-lookup"><span data-stu-id="eeb65-118">Name</span></span>      |<span data-ttu-id="eeb65-119">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb65-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eeb65-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eeb65-120">Authorization</span></span>  | <span data-ttu-id="eeb65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eeb65-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eeb65-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eeb65-123">Request body</span></span>
<span data-ttu-id="eeb65-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eeb65-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeb65-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="eeb65-125">Response</span></span>

<span data-ttu-id="eeb65-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [User](../resources/user.md) или [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eeb65-126">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeb65-127">Пример</span><span class="sxs-lookup"><span data-stu-id="eeb65-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeb65-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="eeb65-128">Request</span></span>
<span data-ttu-id="eeb65-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eeb65-129">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="eeb65-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="eeb65-130">Response</span></span>
<span data-ttu-id="eeb65-131">Ниже приведен пример респоне.</span><span class="sxs-lookup"><span data-stu-id="eeb65-131">Here is an example of the respone.</span></span> <span data-ttu-id="eeb65-132">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="eeb65-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eeb65-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eeb65-133">All of the properties will be returned from an actual call.</span></span>

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
