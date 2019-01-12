---
title: Получение параметров
description: Чтение объекта параметры пользователей и организаций.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5e9f66d96fc0f742196bf97c7e54406231d2b042
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914831"
---
# <a name="get-settings"></a><span data-ttu-id="87524-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="87524-103">Get settings</span></span>

> <span data-ttu-id="87524-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87524-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87524-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87524-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87524-106">Чтение объекта [Параметры](../resources/user-settings.md) пользователей и организаций.</span><span class="sxs-lookup"><span data-stu-id="87524-106">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="87524-107">Чтобы узнать, как обновить свойства объекта [параметров](../resources/user-settings.md) , обратитесь к разделу [Изменение параметров пользователей](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="87524-107">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87524-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87524-108">Permissions</span></span>

<span data-ttu-id="87524-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87524-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87524-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87524-111">Permission type</span></span>      | <span data-ttu-id="87524-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87524-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87524-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87524-113">Delegated (work or school account)</span></span> | <span data-ttu-id="87524-114">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87524-114">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="87524-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87524-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87524-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87524-116">Not supported.</span></span>    |
|<span data-ttu-id="87524-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87524-117">Application</span></span> | <span data-ttu-id="87524-118">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87524-118">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87524-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87524-119">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="87524-120">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="87524-120">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="87524-121">[Для получения дополнительных сведений см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="87524-121">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="87524-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87524-122">Request body</span></span>

<span data-ttu-id="87524-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87524-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87524-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="87524-124">Response</span></span>

<span data-ttu-id="87524-125">Успешно завершена, этот метод возвращает `200 OK` объект [параметров пользователя](../resources/user-settings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87524-125">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87524-126">Пример</span><span class="sxs-lookup"><span data-stu-id="87524-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87524-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="87524-127">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="87524-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="87524-128">Response</span></span>

<span data-ttu-id="87524-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87524-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
