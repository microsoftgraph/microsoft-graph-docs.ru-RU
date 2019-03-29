---
title: Обновление Андроидфорворкапп
description: Обновление свойств объекта Андроидфорворкапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86c2362829ea1b7d7651161992171fef1d4a52a6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963837"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="66483-103">Обновление Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="66483-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="66483-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66483-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66483-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66483-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66483-106">Обновление свойств объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="66483-106">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66483-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="66483-107">Prerequisites</span></span>
<span data-ttu-id="66483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66483-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66483-110">Permission type</span></span>|<span data-ttu-id="66483-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66483-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66483-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66483-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66483-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66483-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66483-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66483-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66483-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66483-115">Not supported.</span></span>|
|<span data-ttu-id="66483-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66483-116">Application</span></span>|<span data-ttu-id="66483-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66483-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66483-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66483-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="66483-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66483-119">Request headers</span></span>
|<span data-ttu-id="66483-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66483-120">Header</span></span>|<span data-ttu-id="66483-121">Значение</span><span class="sxs-lookup"><span data-stu-id="66483-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66483-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66483-122">Authorization</span></span>|<span data-ttu-id="66483-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66483-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66483-124">Accept</span><span class="sxs-lookup"><span data-stu-id="66483-124">Accept</span></span>|<span data-ttu-id="66483-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66483-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66483-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66483-126">Request body</span></span>
<span data-ttu-id="66483-127">В тексте запроса добавьте представление объекта [Андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66483-127">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="66483-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-128">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="66483-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="66483-129">Property</span></span>|<span data-ttu-id="66483-130">Тип</span><span class="sxs-lookup"><span data-stu-id="66483-130">Type</span></span>|<span data-ttu-id="66483-131">Описание</span><span class="sxs-lookup"><span data-stu-id="66483-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66483-132">id</span><span class="sxs-lookup"><span data-stu-id="66483-132">id</span></span>|<span data-ttu-id="66483-133">Строка</span><span class="sxs-lookup"><span data-stu-id="66483-133">String</span></span>|<span data-ttu-id="66483-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="66483-134">Key of the entity.</span></span> <span data-ttu-id="66483-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-136">displayName</span><span class="sxs-lookup"><span data-stu-id="66483-136">displayName</span></span>|<span data-ttu-id="66483-137">Строка</span><span class="sxs-lookup"><span data-stu-id="66483-137">String</span></span>|<span data-ttu-id="66483-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="66483-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="66483-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-140">description</span><span class="sxs-lookup"><span data-stu-id="66483-140">description</span></span>|<span data-ttu-id="66483-141">String</span><span class="sxs-lookup"><span data-stu-id="66483-141">String</span></span>|<span data-ttu-id="66483-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-142">The description of the app.</span></span> <span data-ttu-id="66483-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-144">publisher</span><span class="sxs-lookup"><span data-stu-id="66483-144">publisher</span></span>|<span data-ttu-id="66483-145">String</span><span class="sxs-lookup"><span data-stu-id="66483-145">String</span></span>|<span data-ttu-id="66483-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-146">The publisher of the app.</span></span> <span data-ttu-id="66483-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="66483-148">largeIcon</span></span>|[<span data-ttu-id="66483-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="66483-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="66483-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="66483-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="66483-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66483-152">createdDateTime</span></span>|<span data-ttu-id="66483-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66483-153">DateTimeOffset</span></span>|<span data-ttu-id="66483-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-154">The date and time the app was created.</span></span> <span data-ttu-id="66483-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66483-156">lastModifiedDateTime</span></span>|<span data-ttu-id="66483-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66483-157">DateTimeOffset</span></span>|<span data-ttu-id="66483-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-158">The date and time the app was last modified.</span></span> <span data-ttu-id="66483-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="66483-160">isFeatured</span></span>|<span data-ttu-id="66483-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="66483-161">Boolean</span></span>|<span data-ttu-id="66483-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="66483-163">privacyInformationUrl</span></span>|<span data-ttu-id="66483-164">String</span><span class="sxs-lookup"><span data-stu-id="66483-164">String</span></span>|<span data-ttu-id="66483-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="66483-165">The privacy statement Url.</span></span> <span data-ttu-id="66483-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="66483-167">informationUrl</span></span>|<span data-ttu-id="66483-168">String</span><span class="sxs-lookup"><span data-stu-id="66483-168">String</span></span>|<span data-ttu-id="66483-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="66483-169">The more information Url.</span></span> <span data-ttu-id="66483-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-171">owner</span><span class="sxs-lookup"><span data-stu-id="66483-171">owner</span></span>|<span data-ttu-id="66483-172">String</span><span class="sxs-lookup"><span data-stu-id="66483-172">String</span></span>|<span data-ttu-id="66483-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-173">The owner of the app.</span></span> <span data-ttu-id="66483-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-175">developer</span><span class="sxs-lookup"><span data-stu-id="66483-175">developer</span></span>|<span data-ttu-id="66483-176">String</span><span class="sxs-lookup"><span data-stu-id="66483-176">String</span></span>|<span data-ttu-id="66483-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-177">The developer of the app.</span></span> <span data-ttu-id="66483-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-179">notes</span><span class="sxs-lookup"><span data-stu-id="66483-179">notes</span></span>|<span data-ttu-id="66483-180">String</span><span class="sxs-lookup"><span data-stu-id="66483-180">String</span></span>|<span data-ttu-id="66483-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-181">Notes for the app.</span></span> <span data-ttu-id="66483-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="66483-183">uploadState</span></span>|<span data-ttu-id="66483-184">Int32</span><span class="sxs-lookup"><span data-stu-id="66483-184">Int32</span></span>|<span data-ttu-id="66483-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="66483-185">The upload state.</span></span> <span data-ttu-id="66483-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="66483-187">publishingState</span></span>|[<span data-ttu-id="66483-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="66483-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="66483-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-189">The publishing state for the app.</span></span> <span data-ttu-id="66483-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="66483-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="66483-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="66483-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="66483-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="66483-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="66483-193">isAssigned</span></span>|<span data-ttu-id="66483-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="66483-194">Boolean</span></span>|<span data-ttu-id="66483-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="66483-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="66483-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66483-197">roleScopeTagIds</span></span>|<span data-ttu-id="66483-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="66483-198">String collection</span></span>|<span data-ttu-id="66483-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="66483-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="66483-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66483-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66483-201">packageId</span><span class="sxs-lookup"><span data-stu-id="66483-201">packageId</span></span>|<span data-ttu-id="66483-202">String</span><span class="sxs-lookup"><span data-stu-id="66483-202">String</span></span>|<span data-ttu-id="66483-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="66483-203">The package identifier.</span></span>|
|<span data-ttu-id="66483-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="66483-204">appIdentifier</span></span>|<span data-ttu-id="66483-205">String</span><span class="sxs-lookup"><span data-stu-id="66483-205">String</span></span>|<span data-ttu-id="66483-206">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="66483-206">The Identity Name.</span></span>|
|<span data-ttu-id="66483-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="66483-207">usedLicenseCount</span></span>|<span data-ttu-id="66483-208">Int32</span><span class="sxs-lookup"><span data-stu-id="66483-208">Int32</span></span>|<span data-ttu-id="66483-209">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="66483-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="66483-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="66483-210">totalLicenseCount</span></span>|<span data-ttu-id="66483-211">Int32</span><span class="sxs-lookup"><span data-stu-id="66483-211">Int32</span></span>|<span data-ttu-id="66483-212">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="66483-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="66483-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="66483-213">appStoreUrl</span></span>|<span data-ttu-id="66483-214">String</span><span class="sxs-lookup"><span data-stu-id="66483-214">String</span></span>|<span data-ttu-id="66483-215">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="66483-215">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="66483-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="66483-216">Response</span></span>
<span data-ttu-id="66483-217">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66483-217">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66483-218">Пример</span><span class="sxs-lookup"><span data-stu-id="66483-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="66483-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="66483-219">Request</span></span>
<span data-ttu-id="66483-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66483-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 876

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="66483-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="66483-221">Response</span></span>
<span data-ttu-id="66483-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66483-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




