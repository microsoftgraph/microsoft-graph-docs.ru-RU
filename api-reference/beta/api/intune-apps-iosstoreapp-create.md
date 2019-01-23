---
title: Create iosStoreApp
description: Создание объекта iosStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d08ed1165735f20248a5d9fec85f68bac78fb31
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405788"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="48da0-103">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="48da0-103">Create iosStoreApp</span></span>

> <span data-ttu-id="48da0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48da0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48da0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48da0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48da0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="48da0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48da0-107">Создание объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48da0-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="48da0-108">Prerequisites</span></span>
<span data-ttu-id="48da0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48da0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48da0-111">Permission type</span></span>|<span data-ttu-id="48da0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="48da0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48da0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48da0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48da0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48da0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48da0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48da0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48da0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48da0-116">Not supported.</span></span>|
|<span data-ttu-id="48da0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48da0-117">Application</span></span>|<span data-ttu-id="48da0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48da0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48da0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48da0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="48da0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48da0-120">Request headers</span></span>
|<span data-ttu-id="48da0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48da0-121">Header</span></span>|<span data-ttu-id="48da0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48da0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48da0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="48da0-123">Authorization</span></span>|<span data-ttu-id="48da0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="48da0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48da0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48da0-125">Accept</span></span>|<span data-ttu-id="48da0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48da0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48da0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48da0-127">Request body</span></span>
<span data-ttu-id="48da0-128">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48da0-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="48da0-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="48da0-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="48da0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="48da0-130">Property</span></span>|<span data-ttu-id="48da0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="48da0-131">Type</span></span>|<span data-ttu-id="48da0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="48da0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48da0-133">id</span><span class="sxs-lookup"><span data-stu-id="48da0-133">id</span></span>|<span data-ttu-id="48da0-134">String</span><span class="sxs-lookup"><span data-stu-id="48da0-134">String</span></span>|<span data-ttu-id="48da0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="48da0-135">Key of the entity.</span></span> <span data-ttu-id="48da0-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="48da0-137">displayName</span></span>|<span data-ttu-id="48da0-138">String</span><span class="sxs-lookup"><span data-stu-id="48da0-138">String</span></span>|<span data-ttu-id="48da0-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="48da0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="48da0-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-141">description</span><span class="sxs-lookup"><span data-stu-id="48da0-141">description</span></span>|<span data-ttu-id="48da0-142">String</span><span class="sxs-lookup"><span data-stu-id="48da0-142">String</span></span>|<span data-ttu-id="48da0-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-143">The description of the app.</span></span> <span data-ttu-id="48da0-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="48da0-145">publisher</span></span>|<span data-ttu-id="48da0-146">String</span><span class="sxs-lookup"><span data-stu-id="48da0-146">String</span></span>|<span data-ttu-id="48da0-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-147">The publisher of the app.</span></span> <span data-ttu-id="48da0-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48da0-149">largeIcon</span></span>|[<span data-ttu-id="48da0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48da0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48da0-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="48da0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="48da0-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48da0-153">createdDateTime</span></span>|<span data-ttu-id="48da0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48da0-154">DateTimeOffset</span></span>|<span data-ttu-id="48da0-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-155">The date and time the app was created.</span></span> <span data-ttu-id="48da0-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48da0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="48da0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48da0-158">DateTimeOffset</span></span>|<span data-ttu-id="48da0-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="48da0-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48da0-161">isFeatured</span></span>|<span data-ttu-id="48da0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="48da0-162">Boolean</span></span>|<span data-ttu-id="48da0-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48da0-164">privacyInformationUrl</span></span>|<span data-ttu-id="48da0-165">String</span><span class="sxs-lookup"><span data-stu-id="48da0-165">String</span></span>|<span data-ttu-id="48da0-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="48da0-166">The privacy statement Url.</span></span> <span data-ttu-id="48da0-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48da0-168">informationUrl</span></span>|<span data-ttu-id="48da0-169">String</span><span class="sxs-lookup"><span data-stu-id="48da0-169">String</span></span>|<span data-ttu-id="48da0-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="48da0-170">The more information Url.</span></span> <span data-ttu-id="48da0-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-172">owner</span><span class="sxs-lookup"><span data-stu-id="48da0-172">owner</span></span>|<span data-ttu-id="48da0-173">String</span><span class="sxs-lookup"><span data-stu-id="48da0-173">String</span></span>|<span data-ttu-id="48da0-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-174">The owner of the app.</span></span> <span data-ttu-id="48da0-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-176">developer</span><span class="sxs-lookup"><span data-stu-id="48da0-176">developer</span></span>|<span data-ttu-id="48da0-177">String</span><span class="sxs-lookup"><span data-stu-id="48da0-177">String</span></span>|<span data-ttu-id="48da0-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-178">The developer of the app.</span></span> <span data-ttu-id="48da0-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-180">notes</span><span class="sxs-lookup"><span data-stu-id="48da0-180">notes</span></span>|<span data-ttu-id="48da0-181">String</span><span class="sxs-lookup"><span data-stu-id="48da0-181">String</span></span>|<span data-ttu-id="48da0-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="48da0-182">Notes for the app.</span></span> <span data-ttu-id="48da0-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="48da0-184">uploadState</span></span>|<span data-ttu-id="48da0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="48da0-185">Int32</span></span>|<span data-ttu-id="48da0-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="48da0-186">The upload state.</span></span> <span data-ttu-id="48da0-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="48da0-188">publishingState</span></span>|[<span data-ttu-id="48da0-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48da0-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48da0-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-190">The publishing state for the app.</span></span> <span data-ttu-id="48da0-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="48da0-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48da0-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="48da0-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="48da0-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48da0-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="48da0-194">isAssigned</span></span>|<span data-ttu-id="48da0-195">Логический</span><span class="sxs-lookup"><span data-stu-id="48da0-195">Boolean</span></span>|<span data-ttu-id="48da0-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="48da0-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="48da0-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48da0-198">roleScopeTagIds</span></span>|<span data-ttu-id="48da0-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="48da0-199">String collection</span></span>|<span data-ttu-id="48da0-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="48da0-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="48da0-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48da0-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48da0-202">bundleId</span><span class="sxs-lookup"><span data-stu-id="48da0-202">bundleId</span></span>|<span data-ttu-id="48da0-203">String</span><span class="sxs-lookup"><span data-stu-id="48da0-203">String</span></span>|<span data-ttu-id="48da0-204">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="48da0-204">The Identity Name.</span></span>|
|<span data-ttu-id="48da0-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="48da0-205">appStoreUrl</span></span>|<span data-ttu-id="48da0-206">String</span><span class="sxs-lookup"><span data-stu-id="48da0-206">String</span></span>|<span data-ttu-id="48da0-207">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="48da0-207">The Apple App Store URL</span></span>|
|<span data-ttu-id="48da0-208">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="48da0-208">applicableDeviceType</span></span>|[<span data-ttu-id="48da0-209">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="48da0-209">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="48da0-210">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="48da0-210">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="48da0-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="48da0-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="48da0-212">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="48da0-212">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="48da0-213">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="48da0-213">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="48da0-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="48da0-214">Response</span></span>
<span data-ttu-id="48da0-215">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="48da0-215">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48da0-216">Пример</span><span class="sxs-lookup"><span data-stu-id="48da0-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="48da0-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="48da0-217">Request</span></span>
<span data-ttu-id="48da0-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48da0-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1113

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="48da0-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="48da0-219">Response</span></span>
<span data-ttu-id="48da0-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="48da0-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1285

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```




