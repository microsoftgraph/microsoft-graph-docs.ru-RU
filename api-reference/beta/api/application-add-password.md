---
title: Добавление пароля приложения
description: Добавляет надежный пароль для приложения.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 980f2bdc9d43d5d8e854c92a016d9c40b68d3745
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441573"
---
# <a name="add-application-password"></a><span data-ttu-id="bc842-103">Добавление пароля приложения</span><span class="sxs-lookup"><span data-stu-id="bc842-103">Add application password</span></span>

<span data-ttu-id="bc842-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc842-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc842-105">Добавляет надежный пароль для приложения.</span><span class="sxs-lookup"><span data-stu-id="bc842-105">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc842-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc842-106">Permissions</span></span>
<span data-ttu-id="bc842-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc842-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc842-109">Permission type</span></span>      | <span data-ttu-id="bc842-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc842-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc842-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc842-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc842-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc842-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc842-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc842-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc842-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc842-114">Not supported.</span></span>    |
|<span data-ttu-id="bc842-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc842-115">Application</span></span> | <span data-ttu-id="bc842-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc842-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc842-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc842-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="bc842-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc842-118">Request headers</span></span>
| <span data-ttu-id="bc842-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bc842-119">Name</span></span>       | <span data-ttu-id="bc842-120">Тип</span><span class="sxs-lookup"><span data-stu-id="bc842-120">Type</span></span> | <span data-ttu-id="bc842-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bc842-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc842-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc842-122">Authorization</span></span>  | <span data-ttu-id="bc842-123">string</span><span class="sxs-lookup"><span data-stu-id="bc842-123">string</span></span>  | <span data-ttu-id="bc842-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc842-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc842-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc842-126">Request body</span></span>
<span data-ttu-id="bc842-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc842-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc842-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc842-128">Response</span></span>

<span data-ttu-id="bc842-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект Password в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc842-129">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="bc842-130">Azure AD создает надежный пароль, который возвращается с `secretText` помощью свойства.</span><span class="sxs-lookup"><span data-stu-id="bc842-130">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="bc842-131">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="bc842-131">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="bc842-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bc842-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc842-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc842-133">Request</span></span>
<span data-ttu-id="bc842-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc842-134">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="bc842-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc842-135">Response</span></span>
<span data-ttu-id="bc842-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc842-136">Here is an example of the response.</span></span>

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
