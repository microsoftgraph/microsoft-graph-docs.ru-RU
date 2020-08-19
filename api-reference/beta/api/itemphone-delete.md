---
title: Удаление Итемфоне
description: Удаление объекта Итемфоне из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0c7550f1b8e97fbc1a5efcc5d7e712f2550131a8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808055"
---
# <a name="delete-itemphonenumber"></a><span data-ttu-id="51adb-103">Удаление Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="51adb-103">Delete itemPhoneNumber</span></span>

<span data-ttu-id="51adb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51adb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51adb-105">Удаление объекта [итемфоне](../resources/itemphone.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="51adb-105">Delete an [itemPhone](../resources/itemphone.md) object from the user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="51adb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51adb-106">Permissions</span></span>

<span data-ttu-id="51adb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51adb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51adb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51adb-109">Permission type</span></span>                        | <span data-ttu-id="51adb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51adb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51adb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51adb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="51adb-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="51adb-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="51adb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51adb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51adb-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="51adb-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="51adb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51adb-115">Application</span></span>                            | <span data-ttu-id="51adb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51adb-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="51adb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51adb-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/profile/phones/{itemPhoneId}
DELETE /user/{userId}/profile/phones/{itemPhoneId}
```

## <a name="request-headers"></a><span data-ttu-id="51adb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51adb-118">Request headers</span></span>

|<span data-ttu-id="51adb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="51adb-119">Name</span></span>|<span data-ttu-id="51adb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="51adb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51adb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51adb-121">Authorization</span></span>|<span data-ttu-id="51adb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51adb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51adb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51adb-124">Request body</span></span>

<span data-ttu-id="51adb-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51adb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51adb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="51adb-126">Response</span></span>

<span data-ttu-id="51adb-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="51adb-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="51adb-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="51adb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51adb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="51adb-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_itemphone"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/user/{userId}/profile/phones/{itemPhoneId}
```

### <a name="response"></a><span data-ttu-id="51adb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="51adb-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
