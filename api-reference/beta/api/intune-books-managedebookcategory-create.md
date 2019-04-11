---
title: Создание Манажедебуккатегори
description: Создание нового объекта Манажедебуккатегори.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c63b42f066e2e61a0e54bc3aca4a6d41685dd9bd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807681"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="a6f27-103">Создание Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="a6f27-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="a6f27-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6f27-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6f27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f27-106">Создание нового объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a6f27-106">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6f27-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6f27-107">Prerequisites</span></span>
<span data-ttu-id="a6f27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f27-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6f27-110">Permission type</span></span>|<span data-ttu-id="a6f27-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6f27-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6f27-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6f27-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6f27-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f27-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6f27-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6f27-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6f27-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f27-115">Not supported.</span></span>|
|<span data-ttu-id="a6f27-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6f27-116">Application</span></span>|<span data-ttu-id="a6f27-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f27-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6f27-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6f27-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="a6f27-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6f27-119">Request headers</span></span>
|<span data-ttu-id="a6f27-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6f27-120">Header</span></span>|<span data-ttu-id="a6f27-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a6f27-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6f27-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6f27-122">Authorization</span></span>|<span data-ttu-id="a6f27-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6f27-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6f27-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a6f27-124">Accept</span></span>|<span data-ttu-id="a6f27-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6f27-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f27-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6f27-126">Request body</span></span>
<span data-ttu-id="a6f27-127">В тексте запроса добавьте представление объекта Манажедебуккатегори в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6f27-127">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="a6f27-128">В следующей таблице приведены свойства, необходимые при создании Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="a6f27-128">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="a6f27-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6f27-129">Property</span></span>|<span data-ttu-id="a6f27-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a6f27-130">Type</span></span>|<span data-ttu-id="a6f27-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a6f27-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f27-132">id</span><span class="sxs-lookup"><span data-stu-id="a6f27-132">id</span></span>|<span data-ttu-id="a6f27-133">String</span><span class="sxs-lookup"><span data-stu-id="a6f27-133">String</span></span>|<span data-ttu-id="a6f27-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a6f27-134">The key of the entity.</span></span>|
|<span data-ttu-id="a6f27-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a6f27-135">displayName</span></span>|<span data-ttu-id="a6f27-136">String</span><span class="sxs-lookup"><span data-stu-id="a6f27-136">String</span></span>|<span data-ttu-id="a6f27-137">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a6f27-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="a6f27-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6f27-138">lastModifiedDateTime</span></span>|<span data-ttu-id="a6f27-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6f27-139">DateTimeOffset</span></span>|<span data-ttu-id="a6f27-140">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="a6f27-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a6f27-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6f27-141">Response</span></span>
<span data-ttu-id="a6f27-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6f27-142">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6f27-143">Пример</span><span class="sxs-lookup"><span data-stu-id="a6f27-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6f27-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6f27-144">Request</span></span>
<span data-ttu-id="a6f27-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6f27-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6f27-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6f27-146">Response</span></span>
<span data-ttu-id="a6f27-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6f27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





