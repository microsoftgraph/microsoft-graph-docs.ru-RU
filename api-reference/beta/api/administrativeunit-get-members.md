---
title: Получение члена
description: Используйте этот интерфейс API для получения определенного члена (пользователя или группы) административное подразделение.
ms.openlocfilehash: 741a24434056783c3f008de6fb7694082b393092
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077623"
---
# <a name="get-a-member"></a><span data-ttu-id="06a51-103">Получение члена</span><span class="sxs-lookup"><span data-stu-id="06a51-103">Get a member</span></span>

> <span data-ttu-id="06a51-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06a51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06a51-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06a51-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06a51-106">Используйте этот интерфейс API для получения определенного члена (пользователя или группы) административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="06a51-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="06a51-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06a51-107">Permissions</span></span>
<span data-ttu-id="06a51-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06a51-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06a51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06a51-110">Permission type</span></span>      | <span data-ttu-id="06a51-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06a51-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06a51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06a51-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06a51-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06a51-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06a51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06a51-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06a51-115">Not supported.</span></span>    |
|<span data-ttu-id="06a51-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06a51-116">Application</span></span> | <span data-ttu-id="06a51-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06a51-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06a51-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06a51-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="06a51-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06a51-119">Request headers</span></span>
| <span data-ttu-id="06a51-120">Имя</span><span class="sxs-lookup"><span data-stu-id="06a51-120">Name</span></span>      |<span data-ttu-id="06a51-121">Описание</span><span class="sxs-lookup"><span data-stu-id="06a51-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06a51-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06a51-122">Authorization</span></span>  | <span data-ttu-id="06a51-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06a51-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06a51-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06a51-125">Request body</span></span>
<span data-ttu-id="06a51-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06a51-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06a51-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="06a51-127">Response</span></span>

<span data-ttu-id="06a51-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [пользователя](../resources/user.md) или [группы](../resources/group.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06a51-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a51-129">Пример</span><span class="sxs-lookup"><span data-stu-id="06a51-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06a51-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="06a51-130">Request</span></span>
<span data-ttu-id="06a51-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06a51-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="06a51-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="06a51-132">Response</span></span>
<span data-ttu-id="06a51-133">Ниже приведен пример respone.</span><span class="sxs-lookup"><span data-stu-id="06a51-133">Here is an example of the respone.</span></span> <span data-ttu-id="06a51-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="06a51-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="06a51-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06a51-135">All of the properties will be returned from an actual call.</span></span>

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