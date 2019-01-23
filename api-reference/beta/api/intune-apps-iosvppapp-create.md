---
title: Create iosVppApp
description: Создание объекта iosVppApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8e9ad9c99835a138dc5de52c1008b1e2ba24607f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424541"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="2f51c-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="2f51c-103">Create iosVppApp</span></span>

> <span data-ttu-id="2f51c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f51c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f51c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f51c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f51c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f51c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f51c-107">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f51c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2f51c-108">Prerequisites</span></span>
<span data-ttu-id="2f51c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f51c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f51c-111">Permission type</span></span>|<span data-ttu-id="2f51c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f51c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f51c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f51c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f51c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f51c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f51c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f51c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f51c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f51c-116">Not supported.</span></span>|
|<span data-ttu-id="2f51c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f51c-117">Application</span></span>|<span data-ttu-id="2f51c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f51c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f51c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f51c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2f51c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f51c-120">Request headers</span></span>
|<span data-ttu-id="2f51c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f51c-121">Header</span></span>|<span data-ttu-id="2f51c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f51c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f51c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f51c-123">Authorization</span></span>|<span data-ttu-id="2f51c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f51c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f51c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f51c-125">Accept</span></span>|<span data-ttu-id="2f51c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f51c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f51c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f51c-127">Request body</span></span>
<span data-ttu-id="2f51c-128">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f51c-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="2f51c-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="2f51c-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="2f51c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f51c-130">Property</span></span>|<span data-ttu-id="2f51c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f51c-131">Type</span></span>|<span data-ttu-id="2f51c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f51c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f51c-133">id</span><span class="sxs-lookup"><span data-stu-id="2f51c-133">id</span></span>|<span data-ttu-id="2f51c-134">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-134">String</span></span>|<span data-ttu-id="2f51c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f51c-135">Key of the entity.</span></span> <span data-ttu-id="2f51c-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2f51c-137">displayName</span></span>|<span data-ttu-id="2f51c-138">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-138">String</span></span>|<span data-ttu-id="2f51c-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2f51c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2f51c-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-141">description</span><span class="sxs-lookup"><span data-stu-id="2f51c-141">description</span></span>|<span data-ttu-id="2f51c-142">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-142">String</span></span>|<span data-ttu-id="2f51c-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-143">The description of the app.</span></span> <span data-ttu-id="2f51c-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2f51c-145">publisher</span></span>|<span data-ttu-id="2f51c-146">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-146">String</span></span>|<span data-ttu-id="2f51c-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-147">The publisher of the app.</span></span> <span data-ttu-id="2f51c-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2f51c-149">largeIcon</span></span>|[<span data-ttu-id="2f51c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2f51c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2f51c-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2f51c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2f51c-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f51c-153">createdDateTime</span></span>|<span data-ttu-id="2f51c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f51c-154">DateTimeOffset</span></span>|<span data-ttu-id="2f51c-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-155">The date and time the app was created.</span></span> <span data-ttu-id="2f51c-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f51c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2f51c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f51c-158">DateTimeOffset</span></span>|<span data-ttu-id="2f51c-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2f51c-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2f51c-161">isFeatured</span></span>|<span data-ttu-id="2f51c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f51c-162">Boolean</span></span>|<span data-ttu-id="2f51c-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2f51c-164">privacyInformationUrl</span></span>|<span data-ttu-id="2f51c-165">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-165">String</span></span>|<span data-ttu-id="2f51c-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2f51c-166">The privacy statement Url.</span></span> <span data-ttu-id="2f51c-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2f51c-168">informationUrl</span></span>|<span data-ttu-id="2f51c-169">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-169">String</span></span>|<span data-ttu-id="2f51c-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2f51c-170">The more information Url.</span></span> <span data-ttu-id="2f51c-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-172">owner</span><span class="sxs-lookup"><span data-stu-id="2f51c-172">owner</span></span>|<span data-ttu-id="2f51c-173">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-173">String</span></span>|<span data-ttu-id="2f51c-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-174">The owner of the app.</span></span> <span data-ttu-id="2f51c-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-176">developer</span><span class="sxs-lookup"><span data-stu-id="2f51c-176">developer</span></span>|<span data-ttu-id="2f51c-177">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-177">String</span></span>|<span data-ttu-id="2f51c-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-178">The developer of the app.</span></span> <span data-ttu-id="2f51c-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-180">notes</span><span class="sxs-lookup"><span data-stu-id="2f51c-180">notes</span></span>|<span data-ttu-id="2f51c-181">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-181">String</span></span>|<span data-ttu-id="2f51c-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="2f51c-182">Notes for the app.</span></span> <span data-ttu-id="2f51c-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2f51c-184">uploadState</span></span>|<span data-ttu-id="2f51c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2f51c-185">Int32</span></span>|<span data-ttu-id="2f51c-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="2f51c-186">The upload state.</span></span> <span data-ttu-id="2f51c-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2f51c-188">publishingState</span></span>|[<span data-ttu-id="2f51c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2f51c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2f51c-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-190">The publishing state for the app.</span></span> <span data-ttu-id="2f51c-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2f51c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2f51c-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2f51c-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2f51c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2f51c-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2f51c-194">isAssigned</span></span>|<span data-ttu-id="2f51c-195">Логический</span><span class="sxs-lookup"><span data-stu-id="2f51c-195">Boolean</span></span>|<span data-ttu-id="2f51c-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="2f51c-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2f51c-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f51c-198">roleScopeTagIds</span></span>|<span data-ttu-id="2f51c-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2f51c-199">String collection</span></span>|<span data-ttu-id="2f51c-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2f51c-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f51c-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2f51c-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2f51c-202">usedLicenseCount</span></span>|<span data-ttu-id="2f51c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="2f51c-203">Int32</span></span>|<span data-ttu-id="2f51c-204">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2f51c-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2f51c-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2f51c-205">totalLicenseCount</span></span>|<span data-ttu-id="2f51c-206">Int32</span><span class="sxs-lookup"><span data-stu-id="2f51c-206">Int32</span></span>|<span data-ttu-id="2f51c-207">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2f51c-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2f51c-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="2f51c-208">releaseDateTime</span></span>|<span data-ttu-id="2f51c-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f51c-209">DateTimeOffset</span></span>|<span data-ttu-id="2f51c-210">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="2f51c-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="2f51c-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2f51c-211">appStoreUrl</span></span>|<span data-ttu-id="2f51c-212">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-212">String</span></span>|<span data-ttu-id="2f51c-213">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="2f51c-213">The store URL.</span></span>|
|<span data-ttu-id="2f51c-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="2f51c-214">licensingType</span></span>|[<span data-ttu-id="2f51c-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2f51c-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2f51c-216">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="2f51c-216">The supported License Type.</span></span>|
|<span data-ttu-id="2f51c-217">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2f51c-217">applicableDeviceType</span></span>|[<span data-ttu-id="2f51c-218">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2f51c-218">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2f51c-219">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="2f51c-219">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="2f51c-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2f51c-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="2f51c-221">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-221">String</span></span>|<span data-ttu-id="2f51c-222">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2f51c-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2f51c-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2f51c-223">vppTokenAccountType</span></span>|[<span data-ttu-id="2f51c-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2f51c-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2f51c-225">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2f51c-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2f51c-226">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2f51c-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2f51c-227">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2f51c-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2f51c-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="2f51c-228">vppTokenAppleId</span></span>|<span data-ttu-id="2f51c-229">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-229">String</span></span>|<span data-ttu-id="2f51c-230">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2f51c-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2f51c-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="2f51c-231">bundleId</span></span>|<span data-ttu-id="2f51c-232">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-232">String</span></span>|<span data-ttu-id="2f51c-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-233">The Identity Name.</span></span>|
|<span data-ttu-id="2f51c-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2f51c-234">vppTokenId</span></span>|<span data-ttu-id="2f51c-235">String</span><span class="sxs-lookup"><span data-stu-id="2f51c-235">String</span></span>|<span data-ttu-id="2f51c-236">Идентификатор VPP маркер, связанный с этого приложения.</span><span class="sxs-lookup"><span data-stu-id="2f51c-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="2f51c-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="2f51c-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="2f51c-238">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2f51c-238">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="2f51c-239">Результаты отозвать действия лицензии на это приложение.</span><span class="sxs-lookup"><span data-stu-id="2f51c-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="2f51c-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f51c-240">Response</span></span>
<span data-ttu-id="2f51c-241">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2f51c-241">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f51c-242">Пример</span><span class="sxs-lookup"><span data-stu-id="2f51c-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f51c-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f51c-243">Request</span></span>
<span data-ttu-id="2f51c-244">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f51c-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1972

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="2f51c-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f51c-245">Response</span></span>
<span data-ttu-id="2f51c-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f51c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2144

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




