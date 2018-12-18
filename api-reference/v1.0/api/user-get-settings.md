---
title: Получение параметров
description: Чтение объекта параметры пользователей и организаций.
author: dkershaw10
ms.openlocfilehash: 817cfff56b028e242f0cfb65b966ac6b3173059e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346839"
---
# <a name="get-settings"></a><span data-ttu-id="53461-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="53461-103">Get settings</span></span>

<span data-ttu-id="53461-104">Чтение объекта [Параметры](../resources/user-settings.md) пользователей и организаций.</span><span class="sxs-lookup"><span data-stu-id="53461-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="53461-105">Чтобы узнать, как обновить свойства объекта [параметров](../resources/user-settings.md) , обратитесь к разделу [Изменение параметров пользователей](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="53461-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="53461-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53461-106">Permissions</span></span>

<span data-ttu-id="53461-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53461-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53461-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53461-109">Permission type</span></span>      | <span data-ttu-id="53461-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53461-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53461-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53461-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53461-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53461-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="53461-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53461-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53461-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53461-114">Not supported.</span></span>    |
|<span data-ttu-id="53461-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53461-115">Application</span></span> | <span data-ttu-id="53461-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53461-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53461-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53461-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="53461-118">Запросите с «идентификатор пользователя» или «userPrincipalName» доступен только пользователем или пользователем с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="53461-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="53461-119">[Для получения дополнительных сведений см.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="53461-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="53461-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53461-120">Request body</span></span>

<span data-ttu-id="53461-121">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53461-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53461-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="53461-122">Response</span></span>

<span data-ttu-id="53461-123">Успешно завершена, этот метод возвращает `200 OK` объект [параметров пользователя](../resources/user-settings.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53461-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53461-124">Пример</span><span class="sxs-lookup"><span data-stu-id="53461-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="53461-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="53461-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="53461-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="53461-126">Response</span></span>

<span data-ttu-id="53461-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53461-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

