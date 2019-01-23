---
title: Обновление windowsAppX
description: Обновление свойства объекта windowsAppX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 19deaef0f5cf579fcd92ad2d32dcbf7bf12f0c90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413404"
---
# <a name="update-windowsappx"></a><span data-ttu-id="e3eb4-103">Обновление windowsAppX</span><span class="sxs-lookup"><span data-stu-id="e3eb4-103">Update windowsAppX</span></span>

> <span data-ttu-id="e3eb4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3eb4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3eb4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3eb4-107">Обновление свойства объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="e3eb4-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3eb4-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e3eb4-108">Prerequisites</span></span>
<span data-ttu-id="e3eb4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3eb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3eb4-111">Permission type</span></span>|<span data-ttu-id="e3eb4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3eb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3eb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3eb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3eb4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3eb4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3eb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3eb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3eb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-116">Not supported.</span></span>|
|<span data-ttu-id="e3eb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3eb4-117">Application</span></span>|<span data-ttu-id="e3eb4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3eb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3eb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e3eb4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3eb4-120">Request headers</span></span>
|<span data-ttu-id="e3eb4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3eb4-121">Header</span></span>|<span data-ttu-id="e3eb4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3eb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3eb4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3eb4-123">Authorization</span></span>|<span data-ttu-id="e3eb4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3eb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3eb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3eb4-125">Accept</span></span>|<span data-ttu-id="e3eb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3eb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3eb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3eb4-127">Request body</span></span>
<span data-ttu-id="e3eb4-128">В тексте запроса укажите представление JSON для объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="e3eb4-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="e3eb4-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="e3eb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3eb4-130">Property</span></span>|<span data-ttu-id="e3eb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3eb4-131">Type</span></span>|<span data-ttu-id="e3eb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3eb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3eb4-133">id</span><span class="sxs-lookup"><span data-stu-id="e3eb4-133">id</span></span>|<span data-ttu-id="e3eb4-134">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-134">String</span></span>|<span data-ttu-id="e3eb4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-135">Key of the entity.</span></span> <span data-ttu-id="e3eb4-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e3eb4-137">displayName</span></span>|<span data-ttu-id="e3eb4-138">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-138">String</span></span>|<span data-ttu-id="e3eb4-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e3eb4-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-141">description</span><span class="sxs-lookup"><span data-stu-id="e3eb4-141">description</span></span>|<span data-ttu-id="e3eb4-142">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-142">String</span></span>|<span data-ttu-id="e3eb4-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-143">The description of the app.</span></span> <span data-ttu-id="e3eb4-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e3eb4-145">publisher</span></span>|<span data-ttu-id="e3eb4-146">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-146">String</span></span>|<span data-ttu-id="e3eb4-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-147">The publisher of the app.</span></span> <span data-ttu-id="e3eb4-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e3eb4-149">largeIcon</span></span>|[<span data-ttu-id="e3eb4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3eb4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3eb4-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e3eb4-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3eb4-153">createdDateTime</span></span>|<span data-ttu-id="e3eb4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3eb4-154">DateTimeOffset</span></span>|<span data-ttu-id="e3eb4-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-155">The date and time the app was created.</span></span> <span data-ttu-id="e3eb4-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3eb4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e3eb4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3eb4-158">DateTimeOffset</span></span>|<span data-ttu-id="e3eb4-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e3eb4-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e3eb4-161">isFeatured</span></span>|<span data-ttu-id="e3eb4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3eb4-162">Boolean</span></span>|<span data-ttu-id="e3eb4-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e3eb4-164">privacyInformationUrl</span></span>|<span data-ttu-id="e3eb4-165">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-165">String</span></span>|<span data-ttu-id="e3eb4-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-166">The privacy statement Url.</span></span> <span data-ttu-id="e3eb4-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e3eb4-168">informationUrl</span></span>|<span data-ttu-id="e3eb4-169">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-169">String</span></span>|<span data-ttu-id="e3eb4-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-170">The more information Url.</span></span> <span data-ttu-id="e3eb4-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-172">owner</span><span class="sxs-lookup"><span data-stu-id="e3eb4-172">owner</span></span>|<span data-ttu-id="e3eb4-173">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-173">String</span></span>|<span data-ttu-id="e3eb4-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-174">The owner of the app.</span></span> <span data-ttu-id="e3eb4-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-176">developer</span><span class="sxs-lookup"><span data-stu-id="e3eb4-176">developer</span></span>|<span data-ttu-id="e3eb4-177">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-177">String</span></span>|<span data-ttu-id="e3eb4-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-178">The developer of the app.</span></span> <span data-ttu-id="e3eb4-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-180">notes</span><span class="sxs-lookup"><span data-stu-id="e3eb4-180">notes</span></span>|<span data-ttu-id="e3eb4-181">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-181">String</span></span>|<span data-ttu-id="e3eb4-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-182">Notes for the app.</span></span> <span data-ttu-id="e3eb4-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e3eb4-184">uploadState</span></span>|<span data-ttu-id="e3eb4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e3eb4-185">Int32</span></span>|<span data-ttu-id="e3eb4-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-186">The upload state.</span></span> <span data-ttu-id="e3eb4-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e3eb4-188">publishingState</span></span>|[<span data-ttu-id="e3eb4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e3eb4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e3eb4-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-190">The publishing state for the app.</span></span> <span data-ttu-id="e3eb4-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e3eb4-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e3eb4-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e3eb4-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e3eb4-194">isAssigned</span></span>|<span data-ttu-id="e3eb4-195">Логический</span><span class="sxs-lookup"><span data-stu-id="e3eb4-195">Boolean</span></span>|<span data-ttu-id="e3eb4-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e3eb4-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e3eb4-198">roleScopeTagIds</span></span>|<span data-ttu-id="e3eb4-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-199">String collection</span></span>|<span data-ttu-id="e3eb4-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e3eb4-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3eb4-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e3eb4-202">committedContentVersion</span></span>|<span data-ttu-id="e3eb4-203">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-203">String</span></span>|<span data-ttu-id="e3eb4-204">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-204">The internal committed content version.</span></span> <span data-ttu-id="e3eb4-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e3eb4-206">fileName</span><span class="sxs-lookup"><span data-stu-id="e3eb4-206">fileName</span></span>|<span data-ttu-id="e3eb4-207">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-207">String</span></span>|<span data-ttu-id="e3eb4-208">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-208">The name of the main Lob application file.</span></span> <span data-ttu-id="e3eb4-209">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e3eb4-210">size</span><span class="sxs-lookup"><span data-stu-id="e3eb4-210">size</span></span>|<span data-ttu-id="e3eb4-211">Int64</span><span class="sxs-lookup"><span data-stu-id="e3eb4-211">Int64</span></span>|<span data-ttu-id="e3eb4-212">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="e3eb4-213">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3eb4-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e3eb4-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e3eb4-214">applicableArchitectures</span></span>|[<span data-ttu-id="e3eb4-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e3eb4-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e3eb4-216">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e3eb4-217">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e3eb4-218">identityName</span><span class="sxs-lookup"><span data-stu-id="e3eb4-218">identityName</span></span>|<span data-ttu-id="e3eb4-219">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-219">String</span></span>|<span data-ttu-id="e3eb4-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-220">The Identity Name.</span></span>|
|<span data-ttu-id="e3eb4-221">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e3eb4-221">identityPublisherHash</span></span>|<span data-ttu-id="e3eb4-222">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-222">String</span></span>|<span data-ttu-id="e3eb4-223">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-223">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e3eb4-224">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e3eb4-224">identityResourceIdentifier</span></span>|<span data-ttu-id="e3eb4-225">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-225">String</span></span>|<span data-ttu-id="e3eb4-226">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-226">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e3eb4-227">isBundle</span><span class="sxs-lookup"><span data-stu-id="e3eb4-227">isBundle</span></span>|<span data-ttu-id="e3eb4-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3eb4-228">Boolean</span></span>|<span data-ttu-id="e3eb4-229">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-229">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e3eb4-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e3eb4-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e3eb4-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e3eb4-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e3eb4-232">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e3eb4-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e3eb4-233">identityVersion</span></span>|<span data-ttu-id="e3eb4-234">String</span><span class="sxs-lookup"><span data-stu-id="e3eb4-234">String</span></span>|<span data-ttu-id="e3eb4-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e3eb4-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3eb4-236">Response</span></span>
<span data-ttu-id="e3eb4-237">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAppX](../resources/intune-apps-windowsappx.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-237">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3eb4-238">Пример</span><span class="sxs-lookup"><span data-stu-id="e3eb4-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3eb4-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3eb4-239">Request</span></span>
<span data-ttu-id="e3eb4-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e3eb4-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3eb4-241">Response</span></span>
<span data-ttu-id="e3eb4-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3eb4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```




