---
title: Получение параметров
description: Чтение объекта параметры пользователей и организаций.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 30217d43ac453c9e3502b00ece22ac01edf0abfb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852404"
---
# <a name="get-settings"></a><span data-ttu-id="76c9d-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="76c9d-103">Get settings</span></span>

> <span data-ttu-id="76c9d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="76c9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76c9d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76c9d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76c9d-106">Чтение объекта [Параметры](../resources/user-settings.md) пользователей и организаций.</span><span class="sxs-lookup"><span data-stu-id="76c9d-106">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="76c9d-107">Чтобы узнать, как обновить свойства объекта [параметров](../resources/user-settings.md) , обратитесь к разделу [Изменение параметров пользователей](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="76c9d-107">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76c9d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76c9d-108">Permissions</span></span>

<span data-ttu-id="76c9d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76c9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76c9d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76c9d-111">Permission type</span></span>      | <span data-ttu-id="76c9d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76c9d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76c9d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76c9d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="76c9d-114">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76c9d-114">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="76c9d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76c9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76c9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76c9d-116">Not supported.</span></span>    |
|<span data-ttu-id="76c9d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76c9d-117">Application</span></span> | <span data-ttu-id="76c9d-118">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76c9d-118">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76c9d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76c9d-119">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="76c9d-120">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="76c9d-120">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="76c9d-121">[Для получения дополнительных сведений см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="76c9d-121">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="76c9d-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76c9d-122">Request body</span></span>

<span data-ttu-id="76c9d-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76c9d-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76c9d-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="76c9d-124">Response</span></span>

<span data-ttu-id="76c9d-125">Успешно завершена, этот метод возвращает `200 OK` объект [параметров пользователя](../resources/user-settings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="76c9d-125">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76c9d-126">Пример</span><span class="sxs-lookup"><span data-stu-id="76c9d-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="76c9d-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="76c9d-127">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="76c9d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="76c9d-128">Response</span></span>

<span data-ttu-id="76c9d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="76c9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
