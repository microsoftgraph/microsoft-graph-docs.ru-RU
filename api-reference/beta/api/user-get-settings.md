---
title: Получение параметров
description: Чтение объекта параметров пользователя и Организации.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128feebf624350baaea9fee41c411bd46c2b42c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536577"
---
# <a name="get-settings"></a><span data-ttu-id="316d5-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="316d5-103">Get settings</span></span>

<span data-ttu-id="316d5-104">Чтение объекта [параметров](../resources/user-settings.md) пользователя и Организации.</span><span class="sxs-lookup"><span data-stu-id="316d5-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="316d5-105">Чтобы узнать, как обновить свойства объекта [Settings](../resources/user-settings.md) , ознакомьтесь со статьей [Обновление параметров пользователя](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="316d5-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="316d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="316d5-106">Permissions</span></span>

<span data-ttu-id="316d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="316d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="316d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="316d5-109">Permission type</span></span>      | <span data-ttu-id="316d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="316d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="316d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="316d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="316d5-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="316d5-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="316d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="316d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="316d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="316d5-114">Not supported.</span></span>    |
|<span data-ttu-id="316d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="316d5-115">Application</span></span> | <span data-ttu-id="316d5-116">User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="316d5-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="316d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="316d5-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="316d5-118">Запрос с идентификатором пользователя или userPrincipalName доступен только пользователю или пользователем с разрешениями User. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="316d5-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="316d5-119">Чтобы узнать больше, ознакомьтесь [](/graph/permissions-reference)с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="316d5-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="316d5-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="316d5-120">Request body</span></span>

<span data-ttu-id="316d5-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="316d5-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="316d5-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="316d5-122">Response</span></span>

<span data-ttu-id="316d5-123">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [пользовательских параметров](../resources/user-settings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="316d5-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="316d5-124">Пример</span><span class="sxs-lookup"><span data-stu-id="316d5-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="316d5-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="316d5-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="316d5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="316d5-126">Response</span></span>

<span data-ttu-id="316d5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="316d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

