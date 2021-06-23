---
title: 'cloudPcUserSetting: назначение'
description: Назначение параметров пользователя облачного КОМПЬЮТЕРА группам пользователей.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 66da3f668cc25807ece4a63e51dabe3f5436cf7d
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082092"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="69b07-103">cloudPcUserSetting: назначение</span><span class="sxs-lookup"><span data-stu-id="69b07-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="69b07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69b07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69b07-105">Назначение [cloudPcUserSetting группам](../resources/cloudpcusersetting.md) пользователей.</span><span class="sxs-lookup"><span data-stu-id="69b07-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="69b07-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69b07-106">Permissions</span></span>

<span data-ttu-id="69b07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69b07-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69b07-109">Permission type</span></span>|<span data-ttu-id="69b07-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69b07-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69b07-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69b07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69b07-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b07-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="69b07-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69b07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69b07-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69b07-114">Not supported.</span></span>|
|<span data-ttu-id="69b07-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="69b07-115">Application</span></span>|<span data-ttu-id="69b07-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b07-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69b07-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69b07-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="69b07-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69b07-118">Request headers</span></span>

|<span data-ttu-id="69b07-119">Имя</span><span class="sxs-lookup"><span data-stu-id="69b07-119">Name</span></span>|<span data-ttu-id="69b07-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69b07-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="69b07-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69b07-121">Authorization</span></span>|<span data-ttu-id="69b07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69b07-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="69b07-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69b07-124">Content-Type</span></span>|<span data-ttu-id="69b07-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69b07-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69b07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69b07-127">Request body</span></span>

<span data-ttu-id="69b07-128">В корпусе запроса поставляем представление JSON объекта [cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="69b07-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

|<span data-ttu-id="69b07-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="69b07-129">Parameter</span></span>|<span data-ttu-id="69b07-130">Тип</span><span class="sxs-lookup"><span data-stu-id="69b07-130">Type</span></span>|<span data-ttu-id="69b07-131">Описание</span><span class="sxs-lookup"><span data-stu-id="69b07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69b07-132">assignments</span><span class="sxs-lookup"><span data-stu-id="69b07-132">assignments</span></span>|<span data-ttu-id="69b07-133">[коллекция cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="69b07-133">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) collection</span></span> | <span data-ttu-id="69b07-134">Коллекция пользовательских облачных КОМПЬЮТЕРов, устанавливая ресурсы, которые должны быть назначены соответствующей целевой группе.</span><span class="sxs-lookup"><span data-stu-id="69b07-134">The collection of cloud PC user setting resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="69b07-135">В Microsoft 365 поддерживаются только группы и группы безопасности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69b07-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="69b07-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="69b07-136">Response</span></span>

<span data-ttu-id="69b07-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69b07-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69b07-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="69b07-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69b07-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="69b07-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="69b07-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="69b07-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
