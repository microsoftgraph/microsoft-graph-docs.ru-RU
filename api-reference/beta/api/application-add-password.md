---
title: Добавление приложения пароль
description: Добавляет в приложение надежный пароль.
author: lleonard-msft
ms.openlocfilehash: 88aa499cd478511aacba94c0d28c96592c79a5d5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348743"
---
# <a name="add-application-password"></a><span data-ttu-id="6ecf5-103">Добавление приложения пароль</span><span class="sxs-lookup"><span data-stu-id="6ecf5-103">Add application password</span></span>

> <span data-ttu-id="6ecf5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ecf5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ecf5-106">Добавляет в приложение надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ecf5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecf5-107">Permissions</span></span>
<span data-ttu-id="6ecf5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ecf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ecf5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ecf5-110">Permission type</span></span>      | <span data-ttu-id="6ecf5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ecf5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ecf5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ecf5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6ecf5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ecf5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ecf5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ecf5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ecf5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-115">Not supported.</span></span>    |
|<span data-ttu-id="6ecf5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ecf5-116">Application</span></span> | <span data-ttu-id="6ecf5-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ecf5-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ecf5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ecf5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="6ecf5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ecf5-119">Request headers</span></span>
| <span data-ttu-id="6ecf5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ecf5-120">Name</span></span>       | <span data-ttu-id="6ecf5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6ecf5-121">Type</span></span> | <span data-ttu-id="6ecf5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6ecf5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ecf5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ecf5-123">Authorization</span></span>  | <span data-ttu-id="6ecf5-124">string</span><span class="sxs-lookup"><span data-stu-id="6ecf5-124">string</span></span>  | <span data-ttu-id="6ecf5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6ecf5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ecf5-127">Request body</span></span>
<span data-ttu-id="6ecf5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ecf5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ecf5-129">Response</span></span>

<span data-ttu-id="6ecf5-130">Успешно завершена, этот метод возвращает `200 OK` объект пароль и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="6ecf5-131">Создает надежный пароль, который возвращается с помощью Azure AD `secretText` свойство.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="6ecf5-132">Нет возможности для получения пароля в будущем.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="6ecf5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6ecf5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ecf5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ecf5-134">Request</span></span>
<span data-ttu-id="6ecf5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="6ecf5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ecf5-136">Response</span></span>
<span data-ttu-id="6ecf5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ecf5-137">Here is an example of the response.</span></span>

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
