---
title: Создание Андроидманажедстореапп
description: Создание нового объекта Андроидманажедстореапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aee8b173e7b0a1af7ef730efbb43b3347cdb0162
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572532"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="1d222-103">Создание Андроидманажедстореапп</span><span class="sxs-lookup"><span data-stu-id="1d222-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="1d222-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d222-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d222-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d222-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d222-106">Создание нового объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="1d222-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d222-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d222-107">Prerequisites</span></span>
<span data-ttu-id="1d222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d222-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d222-110">Permission type</span></span>|<span data-ttu-id="1d222-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d222-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d222-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d222-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d222-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d222-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d222-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d222-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d222-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d222-115">Not supported.</span></span>|
|<span data-ttu-id="1d222-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d222-116">Application</span></span>|<span data-ttu-id="1d222-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d222-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d222-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d222-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1d222-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d222-119">Request headers</span></span>
|<span data-ttu-id="1d222-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d222-120">Header</span></span>|<span data-ttu-id="1d222-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1d222-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d222-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d222-122">Authorization</span></span>|<span data-ttu-id="1d222-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d222-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d222-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1d222-124">Accept</span></span>|<span data-ttu-id="1d222-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d222-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d222-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d222-126">Request body</span></span>
<span data-ttu-id="1d222-127">В тексте запроса добавьте представление объекта Андроидманажедстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d222-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="1d222-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореапп.</span><span class="sxs-lookup"><span data-stu-id="1d222-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="1d222-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d222-129">Property</span></span>|<span data-ttu-id="1d222-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1d222-130">Type</span></span>|<span data-ttu-id="1d222-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1d222-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d222-132">id</span><span class="sxs-lookup"><span data-stu-id="1d222-132">id</span></span>|<span data-ttu-id="1d222-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1d222-133">String</span></span>|<span data-ttu-id="1d222-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d222-134">Key of the entity.</span></span> <span data-ttu-id="1d222-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1d222-136">displayName</span></span>|<span data-ttu-id="1d222-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1d222-137">String</span></span>|<span data-ttu-id="1d222-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1d222-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1d222-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-140">description</span><span class="sxs-lookup"><span data-stu-id="1d222-140">description</span></span>|<span data-ttu-id="1d222-141">String</span><span class="sxs-lookup"><span data-stu-id="1d222-141">String</span></span>|<span data-ttu-id="1d222-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-142">The description of the app.</span></span> <span data-ttu-id="1d222-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1d222-144">publisher</span></span>|<span data-ttu-id="1d222-145">String</span><span class="sxs-lookup"><span data-stu-id="1d222-145">String</span></span>|<span data-ttu-id="1d222-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-146">The publisher of the app.</span></span> <span data-ttu-id="1d222-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1d222-148">largeIcon</span></span>|[<span data-ttu-id="1d222-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d222-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1d222-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1d222-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1d222-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d222-152">createdDateTime</span></span>|<span data-ttu-id="1d222-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d222-153">DateTimeOffset</span></span>|<span data-ttu-id="1d222-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-154">The date and time the app was created.</span></span> <span data-ttu-id="1d222-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d222-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1d222-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d222-157">DateTimeOffset</span></span>|<span data-ttu-id="1d222-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1d222-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1d222-160">isFeatured</span></span>|<span data-ttu-id="1d222-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d222-161">Boolean</span></span>|<span data-ttu-id="1d222-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1d222-163">privacyInformationUrl</span></span>|<span data-ttu-id="1d222-164">String</span><span class="sxs-lookup"><span data-stu-id="1d222-164">String</span></span>|<span data-ttu-id="1d222-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1d222-165">The privacy statement Url.</span></span> <span data-ttu-id="1d222-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1d222-167">informationUrl</span></span>|<span data-ttu-id="1d222-168">String</span><span class="sxs-lookup"><span data-stu-id="1d222-168">String</span></span>|<span data-ttu-id="1d222-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1d222-169">The more information Url.</span></span> <span data-ttu-id="1d222-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-171">owner</span><span class="sxs-lookup"><span data-stu-id="1d222-171">owner</span></span>|<span data-ttu-id="1d222-172">String</span><span class="sxs-lookup"><span data-stu-id="1d222-172">String</span></span>|<span data-ttu-id="1d222-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-173">The owner of the app.</span></span> <span data-ttu-id="1d222-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-175">developer</span><span class="sxs-lookup"><span data-stu-id="1d222-175">developer</span></span>|<span data-ttu-id="1d222-176">String</span><span class="sxs-lookup"><span data-stu-id="1d222-176">String</span></span>|<span data-ttu-id="1d222-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-177">The developer of the app.</span></span> <span data-ttu-id="1d222-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-179">notes</span><span class="sxs-lookup"><span data-stu-id="1d222-179">notes</span></span>|<span data-ttu-id="1d222-180">String</span><span class="sxs-lookup"><span data-stu-id="1d222-180">String</span></span>|<span data-ttu-id="1d222-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-181">Notes for the app.</span></span> <span data-ttu-id="1d222-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1d222-183">uploadState</span></span>|<span data-ttu-id="1d222-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1d222-184">Int32</span></span>|<span data-ttu-id="1d222-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="1d222-185">The upload state.</span></span> <span data-ttu-id="1d222-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1d222-187">publishingState</span></span>|[<span data-ttu-id="1d222-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1d222-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1d222-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-189">The publishing state for the app.</span></span> <span data-ttu-id="1d222-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1d222-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1d222-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1d222-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1d222-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1d222-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1d222-193">isAssigned</span></span>|<span data-ttu-id="1d222-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d222-194">Boolean</span></span>|<span data-ttu-id="1d222-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="1d222-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1d222-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d222-197">roleScopeTagIds</span></span>|<span data-ttu-id="1d222-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1d222-198">String collection</span></span>|<span data-ttu-id="1d222-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1d222-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1d222-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d222-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d222-201">packageId</span><span class="sxs-lookup"><span data-stu-id="1d222-201">packageId</span></span>|<span data-ttu-id="1d222-202">String</span><span class="sxs-lookup"><span data-stu-id="1d222-202">String</span></span>|<span data-ttu-id="1d222-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="1d222-203">The package identifier.</span></span>|
|<span data-ttu-id="1d222-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="1d222-204">appIdentifier</span></span>|<span data-ttu-id="1d222-205">String</span><span class="sxs-lookup"><span data-stu-id="1d222-205">String</span></span>|<span data-ttu-id="1d222-206">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="1d222-206">The Identity Name.</span></span>|
|<span data-ttu-id="1d222-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1d222-207">usedLicenseCount</span></span>|<span data-ttu-id="1d222-208">Int32</span><span class="sxs-lookup"><span data-stu-id="1d222-208">Int32</span></span>|<span data-ttu-id="1d222-209">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="1d222-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="1d222-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1d222-210">totalLicenseCount</span></span>|<span data-ttu-id="1d222-211">Int32</span><span class="sxs-lookup"><span data-stu-id="1d222-211">Int32</span></span>|<span data-ttu-id="1d222-212">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="1d222-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="1d222-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1d222-213">appStoreUrl</span></span>|<span data-ttu-id="1d222-214">String</span><span class="sxs-lookup"><span data-stu-id="1d222-214">String</span></span>|<span data-ttu-id="1d222-215">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="1d222-215">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="1d222-216">Суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="1d222-216">supportsOemConfig</span></span>|<span data-ttu-id="1d222-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d222-217">Boolean</span></span>|<span data-ttu-id="1d222-218">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="1d222-218">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1d222-219">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d222-219">Response</span></span>
<span data-ttu-id="1d222-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d222-220">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d222-221">Пример</span><span class="sxs-lookup"><span data-stu-id="1d222-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d222-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d222-222">Request</span></span>
<span data-ttu-id="1d222-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d222-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 911

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="1d222-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d222-224">Response</span></span>
<span data-ttu-id="1d222-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d222-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1083

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```




