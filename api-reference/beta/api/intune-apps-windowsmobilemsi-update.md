---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c1683bff6d0212deff060193aa624f56143246e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409099"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="e5b65-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="e5b65-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="e5b65-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5b65-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5b65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5b65-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5b65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b65-107">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5b65-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5b65-108">Prerequisites</span></span>
<span data-ttu-id="e5b65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e5b65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5b65-111">Permission type</span></span>|<span data-ttu-id="e5b65-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5b65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5b65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5b65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5b65-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b65-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5b65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5b65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5b65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b65-116">Not supported.</span></span>|
|<span data-ttu-id="e5b65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5b65-117">Application</span></span>|<span data-ttu-id="e5b65-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5b65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5b65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e5b65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5b65-120">Request headers</span></span>
|<span data-ttu-id="e5b65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5b65-121">Header</span></span>|<span data-ttu-id="e5b65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5b65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5b65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b65-123">Authorization</span></span>|<span data-ttu-id="e5b65-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e5b65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5b65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5b65-125">Accept</span></span>|<span data-ttu-id="e5b65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5b65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b65-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5b65-127">Request body</span></span>
<span data-ttu-id="e5b65-128">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5b65-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="e5b65-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="e5b65-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5b65-130">Property</span></span>|<span data-ttu-id="e5b65-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5b65-131">Type</span></span>|<span data-ttu-id="e5b65-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5b65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b65-133">id</span><span class="sxs-lookup"><span data-stu-id="e5b65-133">id</span></span>|<span data-ttu-id="e5b65-134">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-134">String</span></span>|<span data-ttu-id="e5b65-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5b65-135">Key of the entity.</span></span> <span data-ttu-id="e5b65-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e5b65-137">displayName</span></span>|<span data-ttu-id="e5b65-138">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-138">String</span></span>|<span data-ttu-id="e5b65-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e5b65-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e5b65-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-141">description</span><span class="sxs-lookup"><span data-stu-id="e5b65-141">description</span></span>|<span data-ttu-id="e5b65-142">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-142">String</span></span>|<span data-ttu-id="e5b65-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-143">The description of the app.</span></span> <span data-ttu-id="e5b65-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e5b65-145">publisher</span></span>|<span data-ttu-id="e5b65-146">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-146">String</span></span>|<span data-ttu-id="e5b65-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-147">The publisher of the app.</span></span> <span data-ttu-id="e5b65-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e5b65-149">largeIcon</span></span>|[<span data-ttu-id="e5b65-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e5b65-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e5b65-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e5b65-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e5b65-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b65-153">createdDateTime</span></span>|<span data-ttu-id="e5b65-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b65-154">DateTimeOffset</span></span>|<span data-ttu-id="e5b65-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-155">The date and time the app was created.</span></span> <span data-ttu-id="e5b65-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b65-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e5b65-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b65-158">DateTimeOffset</span></span>|<span data-ttu-id="e5b65-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e5b65-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e5b65-161">isFeatured</span></span>|<span data-ttu-id="e5b65-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b65-162">Boolean</span></span>|<span data-ttu-id="e5b65-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e5b65-164">privacyInformationUrl</span></span>|<span data-ttu-id="e5b65-165">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-165">String</span></span>|<span data-ttu-id="e5b65-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e5b65-166">The privacy statement Url.</span></span> <span data-ttu-id="e5b65-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e5b65-168">informationUrl</span></span>|<span data-ttu-id="e5b65-169">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-169">String</span></span>|<span data-ttu-id="e5b65-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e5b65-170">The more information Url.</span></span> <span data-ttu-id="e5b65-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-172">owner</span><span class="sxs-lookup"><span data-stu-id="e5b65-172">owner</span></span>|<span data-ttu-id="e5b65-173">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-173">String</span></span>|<span data-ttu-id="e5b65-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-174">The owner of the app.</span></span> <span data-ttu-id="e5b65-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-176">developer</span><span class="sxs-lookup"><span data-stu-id="e5b65-176">developer</span></span>|<span data-ttu-id="e5b65-177">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-177">String</span></span>|<span data-ttu-id="e5b65-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-178">The developer of the app.</span></span> <span data-ttu-id="e5b65-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-180">notes</span><span class="sxs-lookup"><span data-stu-id="e5b65-180">notes</span></span>|<span data-ttu-id="e5b65-181">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-181">String</span></span>|<span data-ttu-id="e5b65-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e5b65-182">Notes for the app.</span></span> <span data-ttu-id="e5b65-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e5b65-184">uploadState</span></span>|<span data-ttu-id="e5b65-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b65-185">Int32</span></span>|<span data-ttu-id="e5b65-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="e5b65-186">The upload state.</span></span> <span data-ttu-id="e5b65-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e5b65-188">publishingState</span></span>|[<span data-ttu-id="e5b65-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e5b65-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e5b65-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-190">The publishing state for the app.</span></span> <span data-ttu-id="e5b65-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e5b65-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e5b65-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e5b65-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e5b65-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e5b65-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e5b65-194">isAssigned</span></span>|<span data-ttu-id="e5b65-195">Логический</span><span class="sxs-lookup"><span data-stu-id="e5b65-195">Boolean</span></span>|<span data-ttu-id="e5b65-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="e5b65-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e5b65-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5b65-198">roleScopeTagIds</span></span>|<span data-ttu-id="e5b65-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5b65-199">String collection</span></span>|<span data-ttu-id="e5b65-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e5b65-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5b65-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e5b65-202">committedContentVersion</span></span>|<span data-ttu-id="e5b65-203">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-203">String</span></span>|<span data-ttu-id="e5b65-204">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e5b65-204">The internal committed content version.</span></span> <span data-ttu-id="e5b65-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5b65-206">fileName</span><span class="sxs-lookup"><span data-stu-id="e5b65-206">fileName</span></span>|<span data-ttu-id="e5b65-207">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-207">String</span></span>|<span data-ttu-id="e5b65-208">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-208">The name of the main Lob application file.</span></span> <span data-ttu-id="e5b65-209">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5b65-210">size</span><span class="sxs-lookup"><span data-stu-id="e5b65-210">size</span></span>|<span data-ttu-id="e5b65-211">Int64</span><span class="sxs-lookup"><span data-stu-id="e5b65-211">Int64</span></span>|<span data-ttu-id="e5b65-212">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e5b65-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="e5b65-213">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5b65-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5b65-214">commandLine</span><span class="sxs-lookup"><span data-stu-id="e5b65-214">commandLine</span></span>|<span data-ttu-id="e5b65-215">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-215">String</span></span>|<span data-ttu-id="e5b65-216">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="e5b65-216">The command line.</span></span>|
|<span data-ttu-id="e5b65-217">productCode</span><span class="sxs-lookup"><span data-stu-id="e5b65-217">productCode</span></span>|<span data-ttu-id="e5b65-218">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-218">String</span></span>|<span data-ttu-id="e5b65-219">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="e5b65-219">The product code.</span></span>|
|<span data-ttu-id="e5b65-220">productVersion</span><span class="sxs-lookup"><span data-stu-id="e5b65-220">productVersion</span></span>|<span data-ttu-id="e5b65-221">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-221">String</span></span>|<span data-ttu-id="e5b65-222">Версия бизнес-приложения MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="e5b65-222">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e5b65-223">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="e5b65-223">ignoreVersionDetection</span></span>|<span data-ttu-id="e5b65-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b65-224">Boolean</span></span>|<span data-ttu-id="e5b65-225">Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e5b65-225">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="e5b65-226">Для бизнес-приложений MSI Windows Mobile с функцией самостоятельного обновления следует использовать значение true.</span><span class="sxs-lookup"><span data-stu-id="e5b65-226">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="e5b65-227">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e5b65-227">identityVersion</span></span>|<span data-ttu-id="e5b65-228">String</span><span class="sxs-lookup"><span data-stu-id="e5b65-228">String</span></span>|<span data-ttu-id="e5b65-229">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-229">The identity version.</span></span>|
|<span data-ttu-id="e5b65-230">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e5b65-230">useDeviceContext</span></span>|<span data-ttu-id="e5b65-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b65-231">Boolean</span></span>|<span data-ttu-id="e5b65-232">Указывает, следует ли установить MSI двумя режимами в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="e5b65-232">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="e5b65-233">Если значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="e5b65-233">If true, app will be installed for all users.</span></span> <span data-ttu-id="e5b65-234">Если задано значение false, приложение будет установлено для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5b65-234">If false, app will be installed per-user.</span></span> <span data-ttu-id="e5b65-235">Если значение null, служба будет использовать пакет MSI контекст установки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e5b65-235">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="e5b65-236">В случае MSI двумя режимами это значение по умолчанию будет пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5b65-236">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="e5b65-237">Не могут задаваться для приложений двумя режимами.</span><span class="sxs-lookup"><span data-stu-id="e5b65-237">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="e5b65-238">Нельзя изменить после первоначального создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b65-238">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="e5b65-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5b65-239">Response</span></span>
<span data-ttu-id="e5b65-240">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5b65-240">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b65-241">Пример</span><span class="sxs-lookup"><span data-stu-id="e5b65-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5b65-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5b65-242">Request</span></span>
<span data-ttu-id="e5b65-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5b65-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="e5b65-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5b65-244">Response</span></span>
<span data-ttu-id="e5b65-p124">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5b65-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




