---
title: Добавление пароля приложения
description: Добавляет надежный пароль для приложения.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d755914128e5945fcd45e2df79fce95f7d5c03df
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107264"
---
# <a name="add-application-password"></a><span data-ttu-id="d2fe0-103">Добавление пароля приложения</span><span class="sxs-lookup"><span data-stu-id="d2fe0-103">Add application password</span></span>

<span data-ttu-id="d2fe0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2fe0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2fe0-105">Добавляет надежный пароль для приложения.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-105">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2fe0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2fe0-106">Permissions</span></span>
<span data-ttu-id="d2fe0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2fe0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2fe0-109">Permission type</span></span>      | <span data-ttu-id="d2fe0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2fe0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2fe0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2fe0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2fe0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2fe0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2fe0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2fe0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2fe0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-114">Not supported.</span></span>    |
|<span data-ttu-id="d2fe0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2fe0-115">Application</span></span> | <span data-ttu-id="d2fe0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2fe0-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2fe0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2fe0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="d2fe0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2fe0-118">Request headers</span></span>
| <span data-ttu-id="d2fe0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2fe0-119">Name</span></span>       | <span data-ttu-id="d2fe0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d2fe0-120">Type</span></span> | <span data-ttu-id="d2fe0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d2fe0-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2fe0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2fe0-122">Authorization</span></span>  | <span data-ttu-id="d2fe0-123">string</span><span class="sxs-lookup"><span data-stu-id="d2fe0-123">string</span></span>  | <span data-ttu-id="d2fe0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2fe0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2fe0-126">Request body</span></span>
<span data-ttu-id="d2fe0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2fe0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2fe0-128">Response</span></span>

<span data-ttu-id="d2fe0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект Password в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-129">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="d2fe0-130">Azure AD создает надежный пароль, который возвращается с `secretText` помощью свойства.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-130">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="d2fe0-131">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-131">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="d2fe0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2fe0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2fe0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2fe0-133">Request</span></span>
<span data-ttu-id="d2fe0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-134">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="d2fe0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2fe0-135">Response</span></span>
<span data-ttu-id="d2fe0-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2fe0-136">Here is an example of the response.</span></span>

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
