---
title: Добавление приложения пароль
description: Добавляет в приложение надежный пароль.
ms.openlocfilehash: 78ccb6cced055ca7f2d2ab201e844a9f50f36939
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075361"
---
# <a name="add-application-password"></a><span data-ttu-id="fcf09-103">Добавление приложения пароль</span><span class="sxs-lookup"><span data-stu-id="fcf09-103">Add application password</span></span>

> <span data-ttu-id="fcf09-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fcf09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcf09-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf09-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fcf09-106">Добавляет в приложение надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="fcf09-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fcf09-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf09-107">Permissions</span></span>
<span data-ttu-id="fcf09-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcf09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcf09-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf09-110">Permission type</span></span>      | <span data-ttu-id="fcf09-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcf09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcf09-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcf09-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fcf09-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fcf09-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fcf09-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcf09-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf09-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf09-115">Not supported.</span></span>    |
|<span data-ttu-id="fcf09-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fcf09-116">Application</span></span> | <span data-ttu-id="fcf09-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcf09-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fcf09-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcf09-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="fcf09-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcf09-119">Request headers</span></span>
| <span data-ttu-id="fcf09-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fcf09-120">Name</span></span>       | <span data-ttu-id="fcf09-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fcf09-121">Type</span></span> | <span data-ttu-id="fcf09-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf09-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcf09-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcf09-123">Authorization</span></span>  | <span data-ttu-id="fcf09-124">string</span><span class="sxs-lookup"><span data-stu-id="fcf09-124">string</span></span>  | <span data-ttu-id="fcf09-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcf09-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fcf09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcf09-127">Request body</span></span>
<span data-ttu-id="fcf09-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcf09-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcf09-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcf09-129">Response</span></span>

<span data-ttu-id="fcf09-130">Успешно завершена, этот метод возвращает `200 OK` объект пароль и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fcf09-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="fcf09-131">Создает надежный пароль, который возвращается с помощью Azure AD `secretText` свойство.</span><span class="sxs-lookup"><span data-stu-id="fcf09-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="fcf09-132">Нет возможности для получения пароля в будущем.</span><span class="sxs-lookup"><span data-stu-id="fcf09-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="fcf09-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fcf09-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcf09-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcf09-134">Request</span></span>
<span data-ttu-id="fcf09-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcf09-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="fcf09-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcf09-136">Response</span></span>
<span data-ttu-id="fcf09-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcf09-137">Here is an example of the response.</span></span>

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
