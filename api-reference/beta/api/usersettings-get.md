---
title: Получение параметров
description: Чтение объекта settings пользователя и организации.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2b69ccc9fd16741d7f758069f73774e85db46c64
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721588"
---
# <a name="get-settings"></a><span data-ttu-id="4d92d-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="4d92d-103">Get settings</span></span>

<span data-ttu-id="4d92d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d92d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d92d-105">Чтение объекта [userSettings](../resources/usersettings.md) пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="4d92d-105">Read the user and organization [userSettings](../resources/usersettings.md) object.</span></span>
<span data-ttu-id="4d92d-106">Сведения об обновлении свойств объекта [userSettings](../resources/usersettings.md) см. в статье [Обновление параметров пользователя](usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="4d92d-106">To learn how to update the properties of the [userSettings](../resources/usersettings.md) object, see [update user settings](usersettings-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d92d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d92d-107">Permissions</span></span>

<span data-ttu-id="4d92d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d92d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d92d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d92d-110">Permission type</span></span>      | <span data-ttu-id="4d92d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d92d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d92d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d92d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4d92d-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d92d-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d92d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d92d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d92d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d92d-115">Not supported.</span></span>    |
|<span data-ttu-id="4d92d-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4d92d-116">Application</span></span> | <span data-ttu-id="4d92d-117">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d92d-117">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d92d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d92d-118">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="4d92d-119">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="4d92d-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="4d92d-120">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d92d-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="4d92d-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d92d-121">Request body</span></span>

<span data-ttu-id="4d92d-122">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d92d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d92d-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d92d-123">Response</span></span>

<span data-ttu-id="4d92d-124">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [userSettings](../resources/usersettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d92d-124">If successful, this method returns a `200 OK` response code and [userSettings](../resources/usersettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d92d-125">Пример</span><span class="sxs-lookup"><span data-stu-id="4d92d-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d92d-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d92d-126">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="4d92d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d92d-127">Response</span></span>

<span data-ttu-id="4d92d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d92d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```


