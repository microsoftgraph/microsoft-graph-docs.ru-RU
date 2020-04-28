---
title: Удаление Алловедусер
description: Отозвать доступ указанного пользователя, чтобы отправить задания печати на связанный общий принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9812f462561a04ffd88e0e927f58b34d963173d4
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43807136"
---
# <a name="delete-alloweduser"></a><span data-ttu-id="01490-103">Удаление Алловедусер</span><span class="sxs-lookup"><span data-stu-id="01490-103">Delete allowedUser</span></span>

<span data-ttu-id="01490-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01490-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01490-105">Отозвать доступ указанного пользователя, чтобы послать задания печати связанному [принтершаре](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="01490-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01490-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01490-106">Permissions</span></span>
<span data-ttu-id="01490-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="01490-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="01490-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="01490-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01490-110">Permission type</span></span> | <span data-ttu-id="01490-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01490-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="01490-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01490-112">Delegated (work or school account)</span></span>| <span data-ttu-id="01490-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="01490-113">Users.Read.All</span></span> |
|<span data-ttu-id="01490-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01490-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01490-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01490-115">Not Supported.</span></span>|
|<span data-ttu-id="01490-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01490-116">Application</span></span>|<span data-ttu-id="01490-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01490-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01490-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01490-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShare/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="01490-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01490-119">Request headers</span></span>
| <span data-ttu-id="01490-120">Имя</span><span class="sxs-lookup"><span data-stu-id="01490-120">Name</span></span>          | <span data-ttu-id="01490-121">Описание</span><span class="sxs-lookup"><span data-stu-id="01490-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="01490-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01490-122">Authorization</span></span> | <span data-ttu-id="01490-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01490-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01490-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01490-125">Request body</span></span>
<span data-ttu-id="01490-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01490-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01490-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="01490-127">Response</span></span>
<span data-ttu-id="01490-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01490-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01490-130">Пример</span><span class="sxs-lookup"><span data-stu-id="01490-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="01490-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="01490-131">Request</span></span>
<span data-ttu-id="01490-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01490-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShare/{id}/allowedUsers/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="01490-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="01490-133">Response</span></span>
<span data-ttu-id="01490-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01490-134">The following is an example of the response.</span></span>
><span data-ttu-id="01490-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01490-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
