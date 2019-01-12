---
title: Создание managedEBookCategory
description: Создание нового объекта managedEBookCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f86f3570f63a6aa3982e9cb2ffbf659d1a9a752c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990252"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="4138c-103">Создание managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="4138c-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="4138c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4138c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4138c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4138c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4138c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4138c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4138c-107">Создание нового объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="4138c-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4138c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4138c-108">Prerequisites</span></span>
<span data-ttu-id="4138c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4138c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4138c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4138c-111">Permission type</span></span>|<span data-ttu-id="4138c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4138c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4138c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4138c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4138c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4138c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4138c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4138c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4138c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4138c-116">Not supported.</span></span>|
|<span data-ttu-id="4138c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4138c-117">Application</span></span>|<span data-ttu-id="4138c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4138c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4138c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4138c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="4138c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4138c-120">Request headers</span></span>
|<span data-ttu-id="4138c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4138c-121">Header</span></span>|<span data-ttu-id="4138c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4138c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4138c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4138c-123">Authorization</span></span>|<span data-ttu-id="4138c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4138c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4138c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4138c-125">Accept</span></span>|<span data-ttu-id="4138c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4138c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4138c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4138c-127">Request body</span></span>
<span data-ttu-id="4138c-128">В тексте запроса укажите представление JSON для объекта managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="4138c-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="4138c-129">В следующей таблице показаны свойства, которые необходимы для создания managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="4138c-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="4138c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4138c-130">Property</span></span>|<span data-ttu-id="4138c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4138c-131">Type</span></span>|<span data-ttu-id="4138c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4138c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4138c-133">id</span><span class="sxs-lookup"><span data-stu-id="4138c-133">id</span></span>|<span data-ttu-id="4138c-134">String</span><span class="sxs-lookup"><span data-stu-id="4138c-134">String</span></span>|<span data-ttu-id="4138c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4138c-135">The key of the entity.</span></span>|
|<span data-ttu-id="4138c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4138c-136">displayName</span></span>|<span data-ttu-id="4138c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4138c-137">String</span></span>|<span data-ttu-id="4138c-138">Имя категории электронная книга.</span><span class="sxs-lookup"><span data-stu-id="4138c-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="4138c-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4138c-139">lastModifiedDateTime</span></span>|<span data-ttu-id="4138c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4138c-140">DateTimeOffset</span></span>|<span data-ttu-id="4138c-141">Дата и время последнего изменения ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="4138c-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="4138c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="4138c-142">Response</span></span>
<span data-ttu-id="4138c-143">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [managedEBookCategory](../resources/intune-books-managedebookcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4138c-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4138c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4138c-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="4138c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4138c-145">Request</span></span>
<span data-ttu-id="4138c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4138c-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4138c-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="4138c-147">Response</span></span>
<span data-ttu-id="4138c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4138c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





