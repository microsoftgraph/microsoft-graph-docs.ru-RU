---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a48ad11974c54e0ec92cefcbaafb5a95349cebd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145782"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="b33a9-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="b33a9-103">Create androidStoreApp</span></span>

> <span data-ttu-id="b33a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b33a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b33a9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b33a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b33a9-106">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b33a9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b33a9-107">Prerequisites</span></span>
<span data-ttu-id="b33a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b33a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b33a9-110">Permission type</span></span>|<span data-ttu-id="b33a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b33a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b33a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b33a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b33a9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b33a9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b33a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b33a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b33a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b33a9-115">Not supported.</span></span>|
|<span data-ttu-id="b33a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b33a9-116">Application</span></span>|<span data-ttu-id="b33a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b33a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b33a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b33a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b33a9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b33a9-119">Request headers</span></span>
|<span data-ttu-id="b33a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b33a9-120">Header</span></span>|<span data-ttu-id="b33a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b33a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b33a9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b33a9-122">Authorization</span></span>|<span data-ttu-id="b33a9-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b33a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b33a9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b33a9-124">Accept</span></span>|<span data-ttu-id="b33a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b33a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b33a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b33a9-126">Request body</span></span>
<span data-ttu-id="b33a9-127">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b33a9-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="b33a9-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="b33a9-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="b33a9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b33a9-129">Property</span></span>|<span data-ttu-id="b33a9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b33a9-130">Type</span></span>|<span data-ttu-id="b33a9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b33a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b33a9-132">id</span><span class="sxs-lookup"><span data-stu-id="b33a9-132">id</span></span>|<span data-ttu-id="b33a9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b33a9-133">String</span></span>|<span data-ttu-id="b33a9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b33a9-134">Key of the entity.</span></span> <span data-ttu-id="b33a9-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b33a9-136">displayName</span></span>|<span data-ttu-id="b33a9-137">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-137">String</span></span>|<span data-ttu-id="b33a9-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b33a9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b33a9-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-140">description</span><span class="sxs-lookup"><span data-stu-id="b33a9-140">description</span></span>|<span data-ttu-id="b33a9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b33a9-141">String</span></span>|<span data-ttu-id="b33a9-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-142">The description of the app.</span></span> <span data-ttu-id="b33a9-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b33a9-144">publisher</span></span>|<span data-ttu-id="b33a9-145">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-145">String</span></span>|<span data-ttu-id="b33a9-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-146">The publisher of the app.</span></span> <span data-ttu-id="b33a9-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b33a9-148">largeIcon</span></span>|[<span data-ttu-id="b33a9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b33a9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b33a9-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b33a9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b33a9-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b33a9-152">createdDateTime</span></span>|<span data-ttu-id="b33a9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b33a9-153">DateTimeOffset</span></span>|<span data-ttu-id="b33a9-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-154">The date and time the app was created.</span></span> <span data-ttu-id="b33a9-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b33a9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b33a9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b33a9-157">DateTimeOffset</span></span>|<span data-ttu-id="b33a9-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b33a9-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b33a9-160">isFeatured</span></span>|<span data-ttu-id="b33a9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b33a9-161">Boolean</span></span>|<span data-ttu-id="b33a9-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b33a9-163">privacyInformationUrl</span></span>|<span data-ttu-id="b33a9-164">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-164">String</span></span>|<span data-ttu-id="b33a9-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b33a9-165">The privacy statement Url.</span></span> <span data-ttu-id="b33a9-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b33a9-167">informationUrl</span></span>|<span data-ttu-id="b33a9-168">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-168">String</span></span>|<span data-ttu-id="b33a9-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b33a9-169">The more information Url.</span></span> <span data-ttu-id="b33a9-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-171">owner</span><span class="sxs-lookup"><span data-stu-id="b33a9-171">owner</span></span>|<span data-ttu-id="b33a9-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b33a9-172">String</span></span>|<span data-ttu-id="b33a9-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-173">The owner of the app.</span></span> <span data-ttu-id="b33a9-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-175">developer</span><span class="sxs-lookup"><span data-stu-id="b33a9-175">developer</span></span>|<span data-ttu-id="b33a9-176">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-176">String</span></span>|<span data-ttu-id="b33a9-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-177">The developer of the app.</span></span> <span data-ttu-id="b33a9-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-179">notes</span><span class="sxs-lookup"><span data-stu-id="b33a9-179">notes</span></span>|<span data-ttu-id="b33a9-180">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-180">String</span></span>|<span data-ttu-id="b33a9-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="b33a9-181">Notes for the app.</span></span> <span data-ttu-id="b33a9-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b33a9-183">uploadState</span></span>|<span data-ttu-id="b33a9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b33a9-184">Int32</span></span>|<span data-ttu-id="b33a9-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b33a9-185">The upload state.</span></span> <span data-ttu-id="b33a9-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b33a9-187">publishingState</span></span>|[<span data-ttu-id="b33a9-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b33a9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b33a9-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-189">The publishing state for the app.</span></span> <span data-ttu-id="b33a9-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b33a9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b33a9-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b33a9-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b33a9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b33a9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b33a9-193">isAssigned</span></span>|<span data-ttu-id="b33a9-194">Логический</span><span class="sxs-lookup"><span data-stu-id="b33a9-194">Boolean</span></span>|<span data-ttu-id="b33a9-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b33a9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b33a9-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b33a9-197">roleScopeTagIds</span></span>|<span data-ttu-id="b33a9-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b33a9-198">String collection</span></span>|<span data-ttu-id="b33a9-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b33a9-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b33a9-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b33a9-201">packageId</span><span class="sxs-lookup"><span data-stu-id="b33a9-201">packageId</span></span>|<span data-ttu-id="b33a9-202">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-202">String</span></span>|<span data-ttu-id="b33a9-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="b33a9-203">The package identifier.</span></span>|
|<span data-ttu-id="b33a9-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="b33a9-204">appIdentifier</span></span>|<span data-ttu-id="b33a9-205">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-205">String</span></span>|<span data-ttu-id="b33a9-206">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b33a9-206">The Identity Name.</span></span>|
|<span data-ttu-id="b33a9-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b33a9-207">appStoreUrl</span></span>|<span data-ttu-id="b33a9-208">String</span><span class="sxs-lookup"><span data-stu-id="b33a9-208">String</span></span>|<span data-ttu-id="b33a9-209">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="b33a9-209">The Android app store URL.</span></span>|
|<span data-ttu-id="b33a9-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b33a9-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b33a9-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b33a9-211">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b33a9-212">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b33a9-212">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b33a9-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="b33a9-213">Response</span></span>
<span data-ttu-id="b33a9-214">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b33a9-214">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b33a9-215">Пример</span><span class="sxs-lookup"><span data-stu-id="b33a9-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="b33a9-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="b33a9-216">Request</span></span>
<span data-ttu-id="b33a9-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b33a9-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1203

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b33a9-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="b33a9-218">Response</span></span>
<span data-ttu-id="b33a9-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b33a9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1375

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




