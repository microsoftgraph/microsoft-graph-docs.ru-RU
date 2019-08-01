---
title: Получение параметров
description: Чтение объекта settings пользователя и организации.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64ecf4c4f44cf59bf3c6344edda7510a6997d813
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027078"
---
# <a name="get-settings"></a><span data-ttu-id="01339-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="01339-103">Get settings</span></span>

<span data-ttu-id="01339-104">Чтение объекта [settings](../resources/user-settings.md) пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="01339-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="01339-105">Сведения об обновлении свойства объекта [settings](../resources/user-settings.md) см. в статье [Обновление параметров пользователя](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="01339-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01339-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01339-106">Permissions</span></span>

<span data-ttu-id="01339-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01339-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01339-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01339-109">Permission type</span></span>      | <span data-ttu-id="01339-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01339-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01339-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01339-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01339-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01339-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="01339-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01339-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01339-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01339-114">Not supported.</span></span>    |
|<span data-ttu-id="01339-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="01339-115">Application</span></span> | <span data-ttu-id="01339-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01339-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01339-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01339-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="01339-118">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="01339-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="01339-119">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01339-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="01339-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01339-120">Request body</span></span>

<span data-ttu-id="01339-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01339-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01339-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="01339-122">Response</span></span>

<span data-ttu-id="01339-123">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user settings](../resources/user-settings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01339-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01339-124">Пример</span><span class="sxs-lookup"><span data-stu-id="01339-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="01339-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="01339-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="01339-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="01339-126">Response</span></span>

<span data-ttu-id="01339-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01339-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

