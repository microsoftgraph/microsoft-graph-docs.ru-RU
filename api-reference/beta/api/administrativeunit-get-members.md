---
title: Получение члена
description: Используйте этот API для получения определенного участника (пользователя или группы) в административном подразделении.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7db3137c8e1862d0b5c8ebf42c8e8a0efac65f27
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991990"
---
# <a name="get-a-member"></a><span data-ttu-id="f39fe-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="f39fe-103">Get a member</span></span>

<span data-ttu-id="f39fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f39fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f39fe-105">Используйте этот API для получения определенного участника (пользователя или группы) в административном подразделении.</span><span class="sxs-lookup"><span data-stu-id="f39fe-105">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="f39fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f39fe-106">Permissions</span></span>
<span data-ttu-id="f39fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f39fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f39fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f39fe-109">Permission type</span></span>      | <span data-ttu-id="f39fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f39fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f39fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f39fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f39fe-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f39fe-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f39fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f39fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f39fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f39fe-114">Not supported.</span></span>    |
|<span data-ttu-id="f39fe-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f39fe-115">Application</span></span> | <span data-ttu-id="f39fe-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f39fe-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f39fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f39fe-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f39fe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f39fe-118">Request headers</span></span>
| <span data-ttu-id="f39fe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f39fe-119">Name</span></span>      |<span data-ttu-id="f39fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f39fe-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f39fe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f39fe-121">Authorization</span></span>  | <span data-ttu-id="f39fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f39fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f39fe-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f39fe-124">Request body</span></span>
<span data-ttu-id="f39fe-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f39fe-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f39fe-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f39fe-126">Response</span></span>

<span data-ttu-id="f39fe-127">В случае успешной работы этот метод возвращает код ответа и объект пользователя или `200 OK` группы в тексте ответа. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="f39fe-127">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f39fe-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f39fe-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f39fe-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f39fe-129">Request</span></span>
<span data-ttu-id="f39fe-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f39fe-130">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="f39fe-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f39fe-131">Response</span></span>
<span data-ttu-id="f39fe-132">Вот пример передыжки.</span><span class="sxs-lookup"><span data-stu-id="f39fe-132">Here is an example of the respone.</span></span> <span data-ttu-id="f39fe-133">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f39fe-133">Note: The response object shown here might be shortened for readability.</span></span>

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


