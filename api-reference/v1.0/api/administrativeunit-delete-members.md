---
title: Удаление участника
description: Используйте этот API для удаления участника (пользователя или группы) из административного подразделения.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 04783b343cd304c666ee03a8872223adef13c2c1
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991605"
---
# <a name="remove-a-member"></a><span data-ttu-id="dac12-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="dac12-103">Remove a member</span></span>

<span data-ttu-id="dac12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dac12-105">Используйте этот API для удаления участника (пользователя или группы) из административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="dac12-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="dac12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dac12-106">Permissions</span></span>
<span data-ttu-id="dac12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dac12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dac12-109">Permission type</span></span>      | <span data-ttu-id="dac12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dac12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dac12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dac12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dac12-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dac12-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dac12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dac12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dac12-114">Not supported.</span></span>    |
|<span data-ttu-id="dac12-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dac12-115">Application</span></span> | <span data-ttu-id="dac12-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac12-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dac12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="dac12-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dac12-118">Request headers</span></span>
| <span data-ttu-id="dac12-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dac12-119">Name</span></span>      |<span data-ttu-id="dac12-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dac12-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dac12-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dac12-121">Authorization</span></span>  | <span data-ttu-id="dac12-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dac12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dac12-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dac12-124">Request body</span></span>
<span data-ttu-id="dac12-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dac12-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dac12-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac12-126">Response</span></span>

<span data-ttu-id="dac12-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dac12-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac12-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dac12-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dac12-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dac12-130">Request</span></span>
<span data-ttu-id="dac12-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dac12-131">Here is an example of the request.</span></span> <span data-ttu-id="dac12-132">В приведенной ниже примере идентификатор id1 представляет идентификатор целевого административного подразделения, а id2 — уникальный идентификатор пользователя или группы членов, которые будут удалены из целевого административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="dac12-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="dac12-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac12-133">Response</span></span>
<span data-ttu-id="dac12-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dac12-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
