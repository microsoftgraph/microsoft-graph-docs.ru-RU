---
title: Обновление windowsPhone81AppX
description: Обновление свойства объекта windowsPhone81AppX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 702fb466edb8437f1455688dc6493d9fbd163e59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401203"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="53bfa-103">Обновление windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="53bfa-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="53bfa-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53bfa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53bfa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53bfa-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53bfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53bfa-107">Обновление свойства объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="53bfa-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53bfa-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="53bfa-108">Prerequisites</span></span>
<span data-ttu-id="53bfa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53bfa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53bfa-111">Permission type</span></span>|<span data-ttu-id="53bfa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53bfa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53bfa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53bfa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53bfa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53bfa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53bfa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53bfa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53bfa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bfa-116">Not supported.</span></span>|
|<span data-ttu-id="53bfa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53bfa-117">Application</span></span>|<span data-ttu-id="53bfa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bfa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53bfa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53bfa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="53bfa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53bfa-120">Request headers</span></span>
|<span data-ttu-id="53bfa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53bfa-121">Header</span></span>|<span data-ttu-id="53bfa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53bfa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53bfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53bfa-123">Authorization</span></span>|<span data-ttu-id="53bfa-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="53bfa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53bfa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53bfa-125">Accept</span></span>|<span data-ttu-id="53bfa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53bfa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53bfa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53bfa-127">Request body</span></span>
<span data-ttu-id="53bfa-128">В тексте запроса укажите представление JSON для объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="53bfa-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="53bfa-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="53bfa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53bfa-130">Property</span></span>|<span data-ttu-id="53bfa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53bfa-131">Type</span></span>|<span data-ttu-id="53bfa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53bfa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bfa-133">id</span><span class="sxs-lookup"><span data-stu-id="53bfa-133">id</span></span>|<span data-ttu-id="53bfa-134">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-134">String</span></span>|<span data-ttu-id="53bfa-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53bfa-135">Key of the entity.</span></span> <span data-ttu-id="53bfa-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="53bfa-137">displayName</span></span>|<span data-ttu-id="53bfa-138">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-138">String</span></span>|<span data-ttu-id="53bfa-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="53bfa-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="53bfa-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-141">description</span><span class="sxs-lookup"><span data-stu-id="53bfa-141">description</span></span>|<span data-ttu-id="53bfa-142">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-142">String</span></span>|<span data-ttu-id="53bfa-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-143">The description of the app.</span></span> <span data-ttu-id="53bfa-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-145">publisher</span><span class="sxs-lookup"><span data-stu-id="53bfa-145">publisher</span></span>|<span data-ttu-id="53bfa-146">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-146">String</span></span>|<span data-ttu-id="53bfa-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-147">The publisher of the app.</span></span> <span data-ttu-id="53bfa-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="53bfa-149">largeIcon</span></span>|[<span data-ttu-id="53bfa-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="53bfa-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="53bfa-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="53bfa-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="53bfa-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53bfa-153">createdDateTime</span></span>|<span data-ttu-id="53bfa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bfa-154">DateTimeOffset</span></span>|<span data-ttu-id="53bfa-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-155">The date and time the app was created.</span></span> <span data-ttu-id="53bfa-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53bfa-157">lastModifiedDateTime</span></span>|<span data-ttu-id="53bfa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53bfa-158">DateTimeOffset</span></span>|<span data-ttu-id="53bfa-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-159">The date and time the app was last modified.</span></span> <span data-ttu-id="53bfa-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="53bfa-161">isFeatured</span></span>|<span data-ttu-id="53bfa-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="53bfa-162">Boolean</span></span>|<span data-ttu-id="53bfa-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="53bfa-164">privacyInformationUrl</span></span>|<span data-ttu-id="53bfa-165">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-165">String</span></span>|<span data-ttu-id="53bfa-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="53bfa-166">The privacy statement Url.</span></span> <span data-ttu-id="53bfa-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="53bfa-168">informationUrl</span></span>|<span data-ttu-id="53bfa-169">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-169">String</span></span>|<span data-ttu-id="53bfa-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="53bfa-170">The more information Url.</span></span> <span data-ttu-id="53bfa-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-172">owner</span><span class="sxs-lookup"><span data-stu-id="53bfa-172">owner</span></span>|<span data-ttu-id="53bfa-173">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-173">String</span></span>|<span data-ttu-id="53bfa-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-174">The owner of the app.</span></span> <span data-ttu-id="53bfa-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-176">developer</span><span class="sxs-lookup"><span data-stu-id="53bfa-176">developer</span></span>|<span data-ttu-id="53bfa-177">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-177">String</span></span>|<span data-ttu-id="53bfa-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-178">The developer of the app.</span></span> <span data-ttu-id="53bfa-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-180">notes</span><span class="sxs-lookup"><span data-stu-id="53bfa-180">notes</span></span>|<span data-ttu-id="53bfa-181">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-181">String</span></span>|<span data-ttu-id="53bfa-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="53bfa-182">Notes for the app.</span></span> <span data-ttu-id="53bfa-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="53bfa-184">uploadState</span></span>|<span data-ttu-id="53bfa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="53bfa-185">Int32</span></span>|<span data-ttu-id="53bfa-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="53bfa-186">The upload state.</span></span> <span data-ttu-id="53bfa-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="53bfa-188">publishingState</span></span>|[<span data-ttu-id="53bfa-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="53bfa-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="53bfa-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-190">The publishing state for the app.</span></span> <span data-ttu-id="53bfa-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="53bfa-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="53bfa-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="53bfa-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="53bfa-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="53bfa-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="53bfa-194">isAssigned</span></span>|<span data-ttu-id="53bfa-195">Логический</span><span class="sxs-lookup"><span data-stu-id="53bfa-195">Boolean</span></span>|<span data-ttu-id="53bfa-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="53bfa-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="53bfa-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53bfa-198">roleScopeTagIds</span></span>|<span data-ttu-id="53bfa-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="53bfa-199">String collection</span></span>|<span data-ttu-id="53bfa-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="53bfa-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53bfa-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="53bfa-202">committedContentVersion</span></span>|<span data-ttu-id="53bfa-203">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-203">String</span></span>|<span data-ttu-id="53bfa-204">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="53bfa-204">The internal committed content version.</span></span> <span data-ttu-id="53bfa-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="53bfa-206">fileName</span><span class="sxs-lookup"><span data-stu-id="53bfa-206">fileName</span></span>|<span data-ttu-id="53bfa-207">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-207">String</span></span>|<span data-ttu-id="53bfa-208">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-208">The name of the main Lob application file.</span></span> <span data-ttu-id="53bfa-209">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="53bfa-210">size</span><span class="sxs-lookup"><span data-stu-id="53bfa-210">size</span></span>|<span data-ttu-id="53bfa-211">Int64</span><span class="sxs-lookup"><span data-stu-id="53bfa-211">Int64</span></span>|<span data-ttu-id="53bfa-212">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="53bfa-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="53bfa-213">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="53bfa-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="53bfa-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="53bfa-214">applicableArchitectures</span></span>|[<span data-ttu-id="53bfa-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="53bfa-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="53bfa-216">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="53bfa-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="53bfa-217">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="53bfa-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="53bfa-218">identityName</span><span class="sxs-lookup"><span data-stu-id="53bfa-218">identityName</span></span>|<span data-ttu-id="53bfa-219">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-219">String</span></span>|<span data-ttu-id="53bfa-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-220">The Identity Name.</span></span>|
|<span data-ttu-id="53bfa-221">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="53bfa-221">identityPublisherHash</span></span>|<span data-ttu-id="53bfa-222">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-222">String</span></span>|<span data-ttu-id="53bfa-223">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="53bfa-223">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="53bfa-224">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="53bfa-224">identityResourceIdentifier</span></span>|<span data-ttu-id="53bfa-225">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-225">String</span></span>|<span data-ttu-id="53bfa-226">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="53bfa-226">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="53bfa-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="53bfa-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="53bfa-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="53bfa-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="53bfa-229">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="53bfa-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="53bfa-230">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="53bfa-230">phoneProductIdentifier</span></span>|<span data-ttu-id="53bfa-231">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-231">String</span></span>|<span data-ttu-id="53bfa-232">Идентификатор продукта телефона.</span><span class="sxs-lookup"><span data-stu-id="53bfa-232">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="53bfa-233">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="53bfa-233">phonePublisherId</span></span>|<span data-ttu-id="53bfa-234">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-234">String</span></span>|<span data-ttu-id="53bfa-235">Publisher с идентификатором телефона.</span><span class="sxs-lookup"><span data-stu-id="53bfa-235">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="53bfa-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="53bfa-236">identityVersion</span></span>|<span data-ttu-id="53bfa-237">String</span><span class="sxs-lookup"><span data-stu-id="53bfa-237">String</span></span>|<span data-ttu-id="53bfa-238">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="53bfa-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="53bfa-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="53bfa-239">Response</span></span>
<span data-ttu-id="53bfa-240">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53bfa-240">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53bfa-241">Пример</span><span class="sxs-lookup"><span data-stu-id="53bfa-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="53bfa-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="53bfa-242">Request</span></span>
<span data-ttu-id="53bfa-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53bfa-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1440

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="53bfa-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="53bfa-244">Response</span></span>
<span data-ttu-id="53bfa-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="53bfa-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1612

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




