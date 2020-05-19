---
title: Добавление пароля приложения
description: Добавляет надежный пароль для приложения.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 944c0a2e30a7202ad85510be84ef8b426059f4b6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289399"
---
# <a name="add-application-password"></a><span data-ttu-id="4fc71-103">Добавление пароля приложения</span><span class="sxs-lookup"><span data-stu-id="4fc71-103">Add application password</span></span>

<span data-ttu-id="4fc71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fc71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fc71-105">Добавляет надежный пароль для приложения.</span><span class="sxs-lookup"><span data-stu-id="4fc71-105">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fc71-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc71-106">Permissions</span></span>
<span data-ttu-id="4fc71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fc71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc71-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc71-109">Permission type</span></span>      | <span data-ttu-id="4fc71-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fc71-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fc71-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fc71-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4fc71-112">Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="4fc71-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4fc71-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fc71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fc71-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fc71-114">Not supported.</span></span>    |
|<span data-ttu-id="4fc71-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fc71-115">Application</span></span> | <span data-ttu-id="4fc71-116">Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4fc71-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fc71-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fc71-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="4fc71-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fc71-118">Request headers</span></span>
| <span data-ttu-id="4fc71-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4fc71-119">Name</span></span>       | <span data-ttu-id="4fc71-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4fc71-120">Type</span></span> | <span data-ttu-id="4fc71-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4fc71-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4fc71-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc71-122">Authorization</span></span>  | <span data-ttu-id="4fc71-123">string</span><span class="sxs-lookup"><span data-stu-id="4fc71-123">string</span></span>  | <span data-ttu-id="4fc71-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fc71-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4fc71-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fc71-126">Request body</span></span>
<span data-ttu-id="4fc71-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fc71-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fc71-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc71-128">Response</span></span>

<span data-ttu-id="4fc71-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект Password в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fc71-129">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="4fc71-130">Azure AD создает надежный пароль, который возвращается с помощью `secretText` Свойства.</span><span class="sxs-lookup"><span data-stu-id="4fc71-130">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="4fc71-131">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="4fc71-131">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="4fc71-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4fc71-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fc71-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fc71-133">Request</span></span>
<span data-ttu-id="4fc71-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fc71-134">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="4fc71-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc71-135">Response</span></span>
<span data-ttu-id="4fc71-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4fc71-136">The following is an example of the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "customKeyIdentifier": "Binary",
    "endDateTime": "String (timestamp)",
    "keyId": "String (identifier)",
    "startDateTime": "String (timestamp)",
    "secretText": "String",
    "hint": "String"
}
```
