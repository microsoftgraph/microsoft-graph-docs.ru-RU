---
title: Добавление приложения пароль
description: Добавляет в приложение надежный пароль.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 15189ee709b2b369d014f9854bcdbd4dc1b7e9be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526825"
---
# <a name="add-application-password"></a><span data-ttu-id="96d65-103">Добавление приложения пароль</span><span class="sxs-lookup"><span data-stu-id="96d65-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96d65-104">Добавляет в приложение надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="96d65-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="96d65-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96d65-105">Permissions</span></span>
<span data-ttu-id="96d65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d65-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96d65-108">Permission type</span></span>      | <span data-ttu-id="96d65-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96d65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96d65-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96d65-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96d65-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96d65-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96d65-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96d65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96d65-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96d65-113">Not supported.</span></span>    |
|<span data-ttu-id="96d65-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96d65-114">Application</span></span> | <span data-ttu-id="96d65-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="96d65-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96d65-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96d65-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="96d65-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96d65-117">Request headers</span></span>
| <span data-ttu-id="96d65-118">Имя</span><span class="sxs-lookup"><span data-stu-id="96d65-118">Name</span></span>       | <span data-ttu-id="96d65-119">Тип</span><span class="sxs-lookup"><span data-stu-id="96d65-119">Type</span></span> | <span data-ttu-id="96d65-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96d65-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96d65-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d65-121">Authorization</span></span>  | <span data-ttu-id="96d65-122">string</span><span class="sxs-lookup"><span data-stu-id="96d65-122">string</span></span>  | <span data-ttu-id="96d65-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96d65-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96d65-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96d65-125">Request body</span></span>
<span data-ttu-id="96d65-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96d65-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96d65-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="96d65-127">Response</span></span>

<span data-ttu-id="96d65-128">Успешно завершена, этот метод возвращает `200 OK` объект пароль и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="96d65-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="96d65-129">Создает надежный пароль, который возвращается с помощью Azure AD `secretText` свойство.</span><span class="sxs-lookup"><span data-stu-id="96d65-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="96d65-130">Нет возможности для получения пароля в будущем.</span><span class="sxs-lookup"><span data-stu-id="96d65-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="96d65-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96d65-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96d65-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96d65-132">Request</span></span>
<span data-ttu-id="96d65-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96d65-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="96d65-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="96d65-134">Response</span></span>
<span data-ttu-id="96d65-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="96d65-135">Here is an example of the response.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/application-add-password.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
