---
title: Добавление участника
description: Используйте этот API, чтобы добавить члена (пользователя или группы) в административную единицу.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef1ff3e00de98a248fbe6a3b059b2de739d7df7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997223"
---
# <a name="add-a-member"></a><span data-ttu-id="3e8a1-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="3e8a1-103">Add a member</span></span>

<span data-ttu-id="3e8a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e8a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e8a1-105">Используйте этот API, чтобы добавить члена (пользователя или группы) в административную единицу.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="3e8a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e8a1-106">Permissions</span></span>
<span data-ttu-id="3e8a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e8a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3e8a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e8a1-109">Permission type</span></span>      | <span data-ttu-id="3e8a1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e8a1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e8a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e8a1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e8a1-112">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="3e8a1-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3e8a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e8a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e8a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-114">Not supported.</span></span>    |
|<span data-ttu-id="3e8a1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e8a1-115">Application</span></span> | <span data-ttu-id="3e8a1-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e8a1-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e8a1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e8a1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3e8a1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e8a1-118">Request headers</span></span>
| <span data-ttu-id="3e8a1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3e8a1-119">Name</span></span>      |<span data-ttu-id="3e8a1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3e8a1-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e8a1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e8a1-121">Authorization</span></span>  | <span data-ttu-id="3e8a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e8a1-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e8a1-124">Request body</span></span>
<span data-ttu-id="3e8a1-125">В тексте запроса укажите `id` [пользователя](../resources/user.md),  [группу](../resources/group.md) или [directoryObject](../resources/directoryobject.md) , которого требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="3e8a1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e8a1-126">Response</span></span>

<span data-ttu-id="3e8a1-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e8a1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3e8a1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e8a1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e8a1-130">Request</span></span>
<span data-ttu-id="3e8a1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-131">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
<span data-ttu-id="3e8a1-132">В тексте запроса укажите `id` объект [пользователя](../resources/user.md) или [группы](../resources/group.md) , который вы хотите добавить.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-132">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

##### <a name="response"></a><span data-ttu-id="3e8a1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e8a1-133">Response</span></span>
<span data-ttu-id="3e8a1-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e8a1-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```


