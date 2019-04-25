---
title: 'Записная книжка: Включеныcopynotebook'
description: Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов. Если эта папка не существует, она будет создана.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: aa684dcaa01f2a8c16be1c75a7b973ee8adb8eea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571732"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="3ecf6-104">Записная книжка: Включеныcopynotebook</span><span class="sxs-lookup"><span data-stu-id="3ecf6-104">notebook: copyNotebook</span></span>
<span data-ttu-id="3ecf6-105">Копирует записную книжку в папку "записные книжки" в библиотеке конечных документов.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-105">Copies a notebook to the Notebooks folder in the destination Documents library.</span></span> <span data-ttu-id="3ecf6-106">Если эта папка не существует, она будет создана.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-106">The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="3ecf6-107">Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ecf6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ecf6-108">Permissions</span></span>
<span data-ttu-id="3ecf6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ecf6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ecf6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ecf6-111">Permission type</span></span>      | <span data-ttu-id="3ecf6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ecf6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ecf6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ecf6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3ecf6-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ecf6-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ecf6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ecf6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ecf6-116">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ecf6-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="3ecf6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ecf6-117">Application</span></span> | <span data-ttu-id="3ecf6-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ecf6-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ecf6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ecf6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="3ecf6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ecf6-120">Request headers</span></span>
| <span data-ttu-id="3ecf6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3ecf6-121">Name</span></span>       | <span data-ttu-id="3ecf6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3ecf6-122">Type</span></span> | <span data-ttu-id="3ecf6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3ecf6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ecf6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ecf6-124">Authorization</span></span>  | <span data-ttu-id="3ecf6-125">string</span><span class="sxs-lookup"><span data-stu-id="3ecf6-125">string</span></span>  | <span data-ttu-id="3ecf6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ecf6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ecf6-128">Content-Type</span></span> | <span data-ttu-id="3ecf6-129">string</span><span class="sxs-lookup"><span data-stu-id="3ecf6-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="3ecf6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ecf6-130">Request body</span></span>
<span data-ttu-id="3ecf6-131">В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span> <span data-ttu-id="3ecf6-132">Вы можете отправить пустой текст, если он не нужен.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-132">It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="3ecf6-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="3ecf6-133">Parameter</span></span>    | <span data-ttu-id="3ecf6-134">Тип</span><span class="sxs-lookup"><span data-stu-id="3ecf6-134">Type</span></span>   |<span data-ttu-id="3ecf6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3ecf6-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ecf6-136">groupId</span><span class="sxs-lookup"><span data-stu-id="3ecf6-136">groupId</span></span>|<span data-ttu-id="3ecf6-137">String</span><span class="sxs-lookup"><span data-stu-id="3ecf6-137">String</span></span>|<span data-ttu-id="3ecf6-138">Идентификатор группы, в которую будет копироваться.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-138">The id of the group to copy to.</span></span> <span data-ttu-id="3ecf6-139">Используйте только при копировании в группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-139">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="3ecf6-140">Ренамеас</span><span class="sxs-lookup"><span data-stu-id="3ecf6-140">renameAs</span></span>|<span data-ttu-id="3ecf6-141">String</span><span class="sxs-lookup"><span data-stu-id="3ecf6-141">String</span></span>|<span data-ttu-id="3ecf6-142">Имя копии.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-142">The name of the copy.</span></span> <span data-ttu-id="3ecf6-143">По умолчанию используется имя существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-143">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="3ecf6-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ecf6-144">Response</span></span>

<span data-ttu-id="3ecf6-145">В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-145">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="3ecf6-146">Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).</span><span class="sxs-lookup"><span data-stu-id="3ecf6-146">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="3ecf6-147">Пример</span><span class="sxs-lookup"><span data-stu-id="3ecf6-147">Example</span></span>
<span data-ttu-id="3ecf6-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3ecf6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ecf6-149">Request</span></span>
<span data-ttu-id="3ecf6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="3ecf6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ecf6-151">Response</span></span>
<span data-ttu-id="3ecf6-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3ecf6-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
