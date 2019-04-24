---
title: Добавление участника
description: Используйте этот API, чтобы добавить члена (пользователя или группы) в административную единицу.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1cc9ce7e091ac96ca2484c74404c3a4b04b19ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459247"
---
# <a name="add-a-member"></a><span data-ttu-id="64a5a-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="64a5a-103">Add a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64a5a-104">Используйте этот API, чтобы добавить члена (пользователя или группы) в административную единицу.</span><span class="sxs-lookup"><span data-stu-id="64a5a-104">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="64a5a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64a5a-105">Permissions</span></span>
<span data-ttu-id="64a5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64a5a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64a5a-108">Permission type</span></span>      | <span data-ttu-id="64a5a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64a5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64a5a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64a5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64a5a-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64a5a-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64a5a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64a5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64a5a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a5a-113">Not supported.</span></span>    |
|<span data-ttu-id="64a5a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64a5a-114">Application</span></span> | <span data-ttu-id="64a5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64a5a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64a5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="64a5a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64a5a-117">Request headers</span></span>
| <span data-ttu-id="64a5a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="64a5a-118">Name</span></span>      |<span data-ttu-id="64a5a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="64a5a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64a5a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64a5a-120">Authorization</span></span>  | <span data-ttu-id="64a5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64a5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64a5a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64a5a-123">Request body</span></span>
<span data-ttu-id="64a5a-124">В тексте запроса добавьте представление объекта [User](../resources/user.md), [Group](../resources/group.md) или [directoryObject](../resources/directoryobject.md) , которое необходимо добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64a5a-124">In the request body, supply a JSON representation of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="64a5a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="64a5a-125">Response</span></span>

<span data-ttu-id="64a5a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="64a5a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64a5a-128">Пример</span><span class="sxs-lookup"><span data-stu-id="64a5a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64a5a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="64a5a-129">Request</span></span>
<span data-ttu-id="64a5a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64a5a-130">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="64a5a-131">В тексте запроса добавьте представление `id` объекта [пользователя](../resources/user.md) или [группы](../resources/group.md) , который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64a5a-131">In the request body, supply a JSON representation of the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="64a5a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="64a5a-132">Response</span></span>
<span data-ttu-id="64a5a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64a5a-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
