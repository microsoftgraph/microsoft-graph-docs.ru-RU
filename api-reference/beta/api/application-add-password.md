---
title: Добавление пароля приложения
description: Добавляет надежный пароль для приложения.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fcd4701b2c9161582b9bd951f35bf0c8ba09821
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945568"
---
# <a name="add-application-password"></a><span data-ttu-id="ee0f3-103">Добавление пароля приложения</span><span class="sxs-lookup"><span data-stu-id="ee0f3-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee0f3-104">Добавляет надежный пароль для приложения.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee0f3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0f3-105">Permissions</span></span>
<span data-ttu-id="ee0f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0f3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee0f3-108">Permission type</span></span>      | <span data-ttu-id="ee0f3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee0f3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee0f3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee0f3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee0f3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee0f3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee0f3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee0f3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee0f3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-113">Not supported.</span></span>    |
|<span data-ttu-id="ee0f3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee0f3-114">Application</span></span> | <span data-ttu-id="ee0f3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee0f3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee0f3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee0f3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="ee0f3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee0f3-117">Request headers</span></span>
| <span data-ttu-id="ee0f3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ee0f3-118">Name</span></span>       | <span data-ttu-id="ee0f3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ee0f3-119">Type</span></span> | <span data-ttu-id="ee0f3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ee0f3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ee0f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee0f3-121">Authorization</span></span>  | <span data-ttu-id="ee0f3-122">string</span><span class="sxs-lookup"><span data-stu-id="ee0f3-122">string</span></span>  | <span data-ttu-id="ee0f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee0f3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee0f3-125">Request body</span></span>
<span data-ttu-id="ee0f3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee0f3-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee0f3-127">Response</span></span>

<span data-ttu-id="ee0f3-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект Password в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="ee0f3-129">Azure AD создает надежный пароль, который возвращается с `secretText` помощью свойства.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="ee0f3-130">В будущем невозможно получить этот пароль.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="ee0f3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ee0f3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee0f3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee0f3-132">Request</span></span>
<span data-ttu-id="ee0f3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="ee0f3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee0f3-134">Response</span></span>
<span data-ttu-id="ee0f3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee0f3-135">Here is an example of the response.</span></span>

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
