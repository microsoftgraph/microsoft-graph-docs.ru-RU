---
title: Создание Андроидфорворкапп
description: Создание нового объекта Андроидфорворкапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c0f589e7955ae5f5663f83ec26b327eea9100a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952466"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="955aa-103">Создание Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="955aa-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="955aa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="955aa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="955aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="955aa-106">Создание нового объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="955aa-106">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="955aa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="955aa-107">Prerequisites</span></span>
<span data-ttu-id="955aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="955aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="955aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="955aa-110">Permission type</span></span>|<span data-ttu-id="955aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="955aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="955aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="955aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="955aa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="955aa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="955aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="955aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="955aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955aa-115">Not supported.</span></span>|
|<span data-ttu-id="955aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="955aa-116">Application</span></span>|<span data-ttu-id="955aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="955aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="955aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="955aa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="955aa-119">Request headers</span></span>
|<span data-ttu-id="955aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="955aa-120">Header</span></span>|<span data-ttu-id="955aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="955aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="955aa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="955aa-122">Authorization</span></span>|<span data-ttu-id="955aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="955aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="955aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="955aa-124">Accept</span></span>|<span data-ttu-id="955aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="955aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="955aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="955aa-126">Request body</span></span>
<span data-ttu-id="955aa-127">В тексте запроса добавьте представление объекта Андроидфорворкапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="955aa-127">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="955aa-128">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкапп.</span><span class="sxs-lookup"><span data-stu-id="955aa-128">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="955aa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="955aa-129">Property</span></span>|<span data-ttu-id="955aa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="955aa-130">Type</span></span>|<span data-ttu-id="955aa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="955aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955aa-132">id</span><span class="sxs-lookup"><span data-stu-id="955aa-132">id</span></span>|<span data-ttu-id="955aa-133">Строка</span><span class="sxs-lookup"><span data-stu-id="955aa-133">String</span></span>|<span data-ttu-id="955aa-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="955aa-134">Key of the entity.</span></span> <span data-ttu-id="955aa-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="955aa-136">displayName</span></span>|<span data-ttu-id="955aa-137">Строка</span><span class="sxs-lookup"><span data-stu-id="955aa-137">String</span></span>|<span data-ttu-id="955aa-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="955aa-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="955aa-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-140">description</span><span class="sxs-lookup"><span data-stu-id="955aa-140">description</span></span>|<span data-ttu-id="955aa-141">Строка</span><span class="sxs-lookup"><span data-stu-id="955aa-141">String</span></span>|<span data-ttu-id="955aa-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-142">The description of the app.</span></span> <span data-ttu-id="955aa-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-144">publisher</span><span class="sxs-lookup"><span data-stu-id="955aa-144">publisher</span></span>|<span data-ttu-id="955aa-145">String</span><span class="sxs-lookup"><span data-stu-id="955aa-145">String</span></span>|<span data-ttu-id="955aa-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-146">The publisher of the app.</span></span> <span data-ttu-id="955aa-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="955aa-148">largeIcon</span></span>|[<span data-ttu-id="955aa-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="955aa-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="955aa-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="955aa-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="955aa-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="955aa-152">createdDateTime</span></span>|<span data-ttu-id="955aa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955aa-153">DateTimeOffset</span></span>|<span data-ttu-id="955aa-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-154">The date and time the app was created.</span></span> <span data-ttu-id="955aa-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="955aa-156">lastModifiedDateTime</span></span>|<span data-ttu-id="955aa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955aa-157">DateTimeOffset</span></span>|<span data-ttu-id="955aa-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-158">The date and time the app was last modified.</span></span> <span data-ttu-id="955aa-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="955aa-160">isFeatured</span></span>|<span data-ttu-id="955aa-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="955aa-161">Boolean</span></span>|<span data-ttu-id="955aa-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="955aa-163">privacyInformationUrl</span></span>|<span data-ttu-id="955aa-164">String</span><span class="sxs-lookup"><span data-stu-id="955aa-164">String</span></span>|<span data-ttu-id="955aa-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="955aa-165">The privacy statement Url.</span></span> <span data-ttu-id="955aa-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="955aa-167">informationUrl</span></span>|<span data-ttu-id="955aa-168">String</span><span class="sxs-lookup"><span data-stu-id="955aa-168">String</span></span>|<span data-ttu-id="955aa-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="955aa-169">The more information Url.</span></span> <span data-ttu-id="955aa-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-171">owner</span><span class="sxs-lookup"><span data-stu-id="955aa-171">owner</span></span>|<span data-ttu-id="955aa-172">String</span><span class="sxs-lookup"><span data-stu-id="955aa-172">String</span></span>|<span data-ttu-id="955aa-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-173">The owner of the app.</span></span> <span data-ttu-id="955aa-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-175">developer</span><span class="sxs-lookup"><span data-stu-id="955aa-175">developer</span></span>|<span data-ttu-id="955aa-176">String</span><span class="sxs-lookup"><span data-stu-id="955aa-176">String</span></span>|<span data-ttu-id="955aa-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-177">The developer of the app.</span></span> <span data-ttu-id="955aa-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-179">notes</span><span class="sxs-lookup"><span data-stu-id="955aa-179">notes</span></span>|<span data-ttu-id="955aa-180">String</span><span class="sxs-lookup"><span data-stu-id="955aa-180">String</span></span>|<span data-ttu-id="955aa-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-181">Notes for the app.</span></span> <span data-ttu-id="955aa-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="955aa-183">uploadState</span></span>|<span data-ttu-id="955aa-184">Int32</span><span class="sxs-lookup"><span data-stu-id="955aa-184">Int32</span></span>|<span data-ttu-id="955aa-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="955aa-185">The upload state.</span></span> <span data-ttu-id="955aa-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="955aa-187">publishingState</span></span>|[<span data-ttu-id="955aa-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="955aa-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="955aa-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-189">The publishing state for the app.</span></span> <span data-ttu-id="955aa-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="955aa-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="955aa-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="955aa-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="955aa-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="955aa-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="955aa-193">isAssigned</span></span>|<span data-ttu-id="955aa-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="955aa-194">Boolean</span></span>|<span data-ttu-id="955aa-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="955aa-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="955aa-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="955aa-197">roleScopeTagIds</span></span>|<span data-ttu-id="955aa-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="955aa-198">String collection</span></span>|<span data-ttu-id="955aa-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="955aa-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="955aa-201">dependentAppCount</span></span>|<span data-ttu-id="955aa-202">Int32</span><span class="sxs-lookup"><span data-stu-id="955aa-202">Int32</span></span>|<span data-ttu-id="955aa-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="955aa-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="955aa-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="955aa-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="955aa-205">packageId</span><span class="sxs-lookup"><span data-stu-id="955aa-205">packageId</span></span>|<span data-ttu-id="955aa-206">String</span><span class="sxs-lookup"><span data-stu-id="955aa-206">String</span></span>|<span data-ttu-id="955aa-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="955aa-207">The package identifier.</span></span>|
|<span data-ttu-id="955aa-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="955aa-208">appIdentifier</span></span>|<span data-ttu-id="955aa-209">String</span><span class="sxs-lookup"><span data-stu-id="955aa-209">String</span></span>|<span data-ttu-id="955aa-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="955aa-210">The Identity Name.</span></span>|
|<span data-ttu-id="955aa-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="955aa-211">usedLicenseCount</span></span>|<span data-ttu-id="955aa-212">Int32</span><span class="sxs-lookup"><span data-stu-id="955aa-212">Int32</span></span>|<span data-ttu-id="955aa-213">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="955aa-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="955aa-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="955aa-214">totalLicenseCount</span></span>|<span data-ttu-id="955aa-215">Int32</span><span class="sxs-lookup"><span data-stu-id="955aa-215">Int32</span></span>|<span data-ttu-id="955aa-216">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="955aa-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="955aa-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="955aa-217">appStoreUrl</span></span>|<span data-ttu-id="955aa-218">String</span><span class="sxs-lookup"><span data-stu-id="955aa-218">String</span></span>|<span data-ttu-id="955aa-219">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="955aa-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="955aa-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="955aa-220">Response</span></span>
<span data-ttu-id="955aa-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="955aa-221">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="955aa-222">Пример</span><span class="sxs-lookup"><span data-stu-id="955aa-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="955aa-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="955aa-223">Request</span></span>
<span data-ttu-id="955aa-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="955aa-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 903

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="955aa-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="955aa-225">Response</span></span>
<span data-ttu-id="955aa-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="955aa-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1075

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





