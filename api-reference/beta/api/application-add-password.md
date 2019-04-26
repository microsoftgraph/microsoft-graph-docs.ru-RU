---
title: Добавление пароля приложения
description: Добавляет надежный пароль для приложения.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dc1e0ebb215ef478c9eedbb44a0d328f35693972
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322658"
---
# <a name="add-application-password"></a><span data-ttu-id="7f17e-103">Добавление пароля приложения</span><span class="sxs-lookup"><span data-stu-id="7f17e-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f17e-104">Добавляет надежный пароль для приложения.</span><span class="sxs-lookup"><span data-stu-id="7f17e-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f17e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f17e-105">Permissions</span></span>
<span data-ttu-id="7f17e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f17e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f17e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f17e-108">Permission type</span></span>      | <span data-ttu-id="7f17e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f17e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f17e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f17e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f17e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f17e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f17e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f17e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f17e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f17e-113">Not supported.</span></span>    |
|<span data-ttu-id="7f17e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f17e-114">Application</span></span> | <span data-ttu-id="7f17e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f17e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f17e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f17e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="7f17e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f17e-117">Request headers</span></span>
| <span data-ttu-id="7f17e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7f17e-118">Name</span></span>       | <span data-ttu-id="7f17e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7f17e-119">Type</span></span> | <span data-ttu-id="7f17e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7f17e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f17e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f17e-121">Authorization</span></span>  | <span data-ttu-id="7f17e-122">string</span><span class="sxs-lookup"><span data-stu-id="7f17e-122">string</span></span>  | <span data-ttu-id="7f17e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f17e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f17e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f17e-125">Request body</span></span>
<span data-ttu-id="7f17e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f17e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f17e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f17e-127">Response</span></span>

<span data-ttu-id="7f17e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект Password в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f17e-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="7f17e-129">Azure AD создает надежный пароль, который возвращается с `secretText` помощью свойства.</span><span class="sxs-lookup"><span data-stu-id="7f17e-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="7f17e-130">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="7f17e-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="7f17e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7f17e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f17e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f17e-132">Request</span></span>
<span data-ttu-id="7f17e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f17e-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="7f17e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f17e-134">Response</span></span>
<span data-ttu-id="7f17e-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f17e-135">Here is an example of the response.</span></span>

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
