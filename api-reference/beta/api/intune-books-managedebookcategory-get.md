---
title: Получение managedEBookCategory
description: Чтение свойства и связи объекта managedEBookCategory.
author: tfitzmac
ms.openlocfilehash: 3a3ece59025b28ed26ffa03931d1de67c45ed140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321961"
---
# <a name="get-managedebookcategory"></a><span data-ttu-id="8f622-103">Получение managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="8f622-103">Get managedEBookCategory</span></span>

> <span data-ttu-id="8f622-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f622-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f622-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f622-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f622-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f622-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f622-107">Чтение свойства и связи объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8f622-107">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f622-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f622-108">Prerequisites</span></span>
<span data-ttu-id="8f622-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f622-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f622-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f622-111">Permission type</span></span>|<span data-ttu-id="8f622-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f622-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f622-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f622-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f622-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f622-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f622-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f622-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f622-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f622-116">Not supported.</span></span>|
|<span data-ttu-id="8f622-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f622-117">Application</span></span>|<span data-ttu-id="8f622-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f622-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f622-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f622-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f622-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8f622-120">Optional query parameters</span></span>
<span data-ttu-id="8f622-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8f622-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8f622-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f622-122">Request headers</span></span>
|<span data-ttu-id="8f622-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f622-123">Header</span></span>|<span data-ttu-id="8f622-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8f622-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f622-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f622-125">Authorization</span></span>|<span data-ttu-id="8f622-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f622-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f622-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8f622-127">Accept</span></span>|<span data-ttu-id="8f622-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8f622-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f622-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f622-129">Request body</span></span>
<span data-ttu-id="8f622-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f622-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f622-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f622-131">Response</span></span>
<span data-ttu-id="8f622-132">Успешно завершена, этот метод возвращает `200 OK` объект [managedEBookCategory](../resources/intune-books-managedebookcategory.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8f622-132">If successful, this method returns a `200 OK` response code and [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f622-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8f622-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f622-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f622-134">Request</span></span>
<span data-ttu-id="8f622-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f622-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
```

### <a name="response"></a><span data-ttu-id="8f622-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f622-136">Response</span></span>
<span data-ttu-id="8f622-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f622-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookCategory",
    "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





