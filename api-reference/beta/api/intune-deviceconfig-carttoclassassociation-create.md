---
title: Создание cartToClassAssociation
description: Создание нового объекта cartToClassAssociation.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 81efbb2c9c06b9a07b1af9ce8f796dd5325ad5fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925478"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="2b208-103">Создание cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="2b208-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="2b208-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b208-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b208-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b208-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b208-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b208-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b208-107">Создание нового объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .</span><span class="sxs-lookup"><span data-stu-id="2b208-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b208-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b208-108">Prerequisites</span></span>
<span data-ttu-id="2b208-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b208-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b208-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b208-111">Permission type</span></span>|<span data-ttu-id="2b208-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b208-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b208-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b208-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b208-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b208-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b208-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b208-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b208-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b208-116">Not supported.</span></span>|
|<span data-ttu-id="2b208-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b208-117">Application</span></span>|<span data-ttu-id="2b208-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b208-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b208-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b208-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="2b208-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b208-120">Request headers</span></span>
|<span data-ttu-id="2b208-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b208-121">Header</span></span>|<span data-ttu-id="2b208-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b208-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b208-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b208-123">Authorization</span></span>|<span data-ttu-id="2b208-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b208-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b208-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b208-125">Accept</span></span>|<span data-ttu-id="2b208-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b208-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b208-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b208-127">Request body</span></span>
<span data-ttu-id="2b208-128">В тексте запроса укажите представление JSON для объекта cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2b208-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="2b208-129">В следующей таблице показаны свойства, которые необходимы для создания cartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2b208-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="2b208-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b208-130">Property</span></span>|<span data-ttu-id="2b208-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b208-131">Type</span></span>|<span data-ttu-id="2b208-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b208-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b208-133">id</span><span class="sxs-lookup"><span data-stu-id="2b208-133">id</span></span>|<span data-ttu-id="2b208-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2b208-134">String</span></span>|<span data-ttu-id="2b208-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b208-135">Key of the entity.</span></span>|
|<span data-ttu-id="2b208-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b208-136">createdDateTime</span></span>|<span data-ttu-id="2b208-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b208-137">DateTimeOffset</span></span>|<span data-ttu-id="2b208-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2b208-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="2b208-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b208-139">lastModifiedDateTime</span></span>|<span data-ttu-id="2b208-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b208-140">DateTimeOffset</span></span>|<span data-ttu-id="2b208-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2b208-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2b208-142">version</span><span class="sxs-lookup"><span data-stu-id="2b208-142">version</span></span>|<span data-ttu-id="2b208-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2b208-143">Int32</span></span>|<span data-ttu-id="2b208-144">Версия CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2b208-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="2b208-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2b208-145">displayName</span></span>|<span data-ttu-id="2b208-146">Строка</span><span class="sxs-lookup"><span data-stu-id="2b208-146">String</span></span>|<span data-ttu-id="2b208-147">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b208-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="2b208-148">описание</span><span class="sxs-lookup"><span data-stu-id="2b208-148">description</span></span>|<span data-ttu-id="2b208-149">Строка</span><span class="sxs-lookup"><span data-stu-id="2b208-149">String</span></span>|<span data-ttu-id="2b208-150">Admin, предоставляемые описание CartToClassAssociation.</span><span class="sxs-lookup"><span data-stu-id="2b208-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="2b208-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="2b208-151">deviceCartIds</span></span>|<span data-ttu-id="2b208-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b208-152">String collection</span></span>|<span data-ttu-id="2b208-153">Идентификаторы корзины устройства необходимо сопоставить с классы.</span><span class="sxs-lookup"><span data-stu-id="2b208-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="2b208-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="2b208-154">classroomIds</span></span>|<span data-ttu-id="2b208-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b208-155">String collection</span></span>|<span data-ttu-id="2b208-156">Идентификаторы аудиторий необходимо сопоставить с устройства корзины.</span><span class="sxs-lookup"><span data-stu-id="2b208-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="2b208-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b208-157">Response</span></span>
<span data-ttu-id="2b208-158">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b208-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b208-159">Пример</span><span class="sxs-lookup"><span data-stu-id="2b208-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b208-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b208-160">Request</span></span>
<span data-ttu-id="2b208-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b208-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="2b208-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b208-162">Response</span></span>
<span data-ttu-id="2b208-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b208-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```





