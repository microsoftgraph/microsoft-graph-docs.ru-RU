---
title: Удаление параметров каталога
description: Удалите параметр каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bebe1604de27b7bfebededd5a470d402f0a36e55
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975444"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="97337-103">Удаление параметров каталога</span><span class="sxs-lookup"><span data-stu-id="97337-103">Delete a directory setting</span></span>

> <span data-ttu-id="97337-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97337-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97337-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97337-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97337-106">Удалите параметр каталога.</span><span class="sxs-lookup"><span data-stu-id="97337-106">Delete a directory setting.</span></span>

> <span data-ttu-id="97337-107">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="97337-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="97337-108">Для *удаления groupSettings*переименован версии /v1.0 этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="97337-108">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="97337-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97337-109">Permissions</span></span>
<span data-ttu-id="97337-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97337-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97337-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97337-112">Permission type</span></span>      | <span data-ttu-id="97337-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97337-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97337-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97337-114">Delegated (work or school account)</span></span> | <span data-ttu-id="97337-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97337-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97337-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97337-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97337-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97337-117">Not supported.</span></span>    |
|<span data-ttu-id="97337-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97337-118">Application</span></span> | <span data-ttu-id="97337-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97337-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97337-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97337-120">HTTP request</span></span>
<span data-ttu-id="97337-121"><!-- { "blockType": "ignored" } -->Удаление конкретных всей клиента или параметр групповой</span><span class="sxs-lookup"><span data-stu-id="97337-121"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="97337-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97337-122">Request headers</span></span>
| <span data-ttu-id="97337-123">Имя</span><span class="sxs-lookup"><span data-stu-id="97337-123">Name</span></span>       | <span data-ttu-id="97337-124">Описание</span><span class="sxs-lookup"><span data-stu-id="97337-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97337-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97337-125">Authorization</span></span>  | <span data-ttu-id="97337-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97337-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97337-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97337-128">Request body</span></span>
<span data-ttu-id="97337-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97337-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97337-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="97337-130">Response</span></span>

<span data-ttu-id="97337-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="97337-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97337-133">Пример</span><span class="sxs-lookup"><span data-stu-id="97337-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97337-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="97337-134">Request</span></span>
<span data-ttu-id="97337-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97337-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="97337-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="97337-136">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
