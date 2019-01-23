---
title: Создание win32LobApp
description: Создание нового объекта win32LobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 089f84f3578c70e3d83b9f7bbfae11e2e72e1eab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409029"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="7a324-103">Создание win32LobApp</span><span class="sxs-lookup"><span data-stu-id="7a324-103">Create win32LobApp</span></span>

> <span data-ttu-id="7a324-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7a324-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a324-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a324-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a324-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a324-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a324-107">Создание нового объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7a324-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a324-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7a324-108">Prerequisites</span></span>
<span data-ttu-id="7a324-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7a324-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a324-111">Permission type</span></span>|<span data-ttu-id="7a324-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a324-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a324-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a324-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a324-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7a324-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a324-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a324-116">Not supported.</span></span>|
|<span data-ttu-id="7a324-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a324-117">Application</span></span>|<span data-ttu-id="7a324-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a324-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a324-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7a324-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a324-120">Request headers</span></span>
|<span data-ttu-id="7a324-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a324-121">Header</span></span>|<span data-ttu-id="7a324-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a324-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a324-123">Authorization</span></span>|<span data-ttu-id="7a324-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7a324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a324-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a324-125">Accept</span></span>|<span data-ttu-id="7a324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a324-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a324-127">Request body</span></span>
<span data-ttu-id="7a324-128">В тексте запроса укажите представление JSON для объекта win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="7a324-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="7a324-129">В следующей таблице показаны свойства, которые необходимы для создания win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="7a324-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="7a324-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a324-130">Property</span></span>|<span data-ttu-id="7a324-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a324-131">Type</span></span>|<span data-ttu-id="7a324-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a324-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a324-133">id</span><span class="sxs-lookup"><span data-stu-id="7a324-133">id</span></span>|<span data-ttu-id="7a324-134">String</span><span class="sxs-lookup"><span data-stu-id="7a324-134">String</span></span>|<span data-ttu-id="7a324-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7a324-135">Key of the entity.</span></span> <span data-ttu-id="7a324-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7a324-137">displayName</span></span>|<span data-ttu-id="7a324-138">String</span><span class="sxs-lookup"><span data-stu-id="7a324-138">String</span></span>|<span data-ttu-id="7a324-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7a324-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7a324-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-141">description</span><span class="sxs-lookup"><span data-stu-id="7a324-141">description</span></span>|<span data-ttu-id="7a324-142">String</span><span class="sxs-lookup"><span data-stu-id="7a324-142">String</span></span>|<span data-ttu-id="7a324-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-143">The description of the app.</span></span> <span data-ttu-id="7a324-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7a324-145">publisher</span></span>|<span data-ttu-id="7a324-146">String</span><span class="sxs-lookup"><span data-stu-id="7a324-146">String</span></span>|<span data-ttu-id="7a324-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-147">The publisher of the app.</span></span> <span data-ttu-id="7a324-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7a324-149">largeIcon</span></span>|[<span data-ttu-id="7a324-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7a324-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7a324-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7a324-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7a324-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a324-153">createdDateTime</span></span>|<span data-ttu-id="7a324-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a324-154">DateTimeOffset</span></span>|<span data-ttu-id="7a324-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-155">The date and time the app was created.</span></span> <span data-ttu-id="7a324-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a324-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7a324-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a324-158">DateTimeOffset</span></span>|<span data-ttu-id="7a324-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7a324-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7a324-161">isFeatured</span></span>|<span data-ttu-id="7a324-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a324-162">Boolean</span></span>|<span data-ttu-id="7a324-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7a324-164">privacyInformationUrl</span></span>|<span data-ttu-id="7a324-165">String</span><span class="sxs-lookup"><span data-stu-id="7a324-165">String</span></span>|<span data-ttu-id="7a324-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7a324-166">The privacy statement Url.</span></span> <span data-ttu-id="7a324-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7a324-168">informationUrl</span></span>|<span data-ttu-id="7a324-169">String</span><span class="sxs-lookup"><span data-stu-id="7a324-169">String</span></span>|<span data-ttu-id="7a324-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7a324-170">The more information Url.</span></span> <span data-ttu-id="7a324-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-172">owner</span><span class="sxs-lookup"><span data-stu-id="7a324-172">owner</span></span>|<span data-ttu-id="7a324-173">String</span><span class="sxs-lookup"><span data-stu-id="7a324-173">String</span></span>|<span data-ttu-id="7a324-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-174">The owner of the app.</span></span> <span data-ttu-id="7a324-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-176">developer</span><span class="sxs-lookup"><span data-stu-id="7a324-176">developer</span></span>|<span data-ttu-id="7a324-177">String</span><span class="sxs-lookup"><span data-stu-id="7a324-177">String</span></span>|<span data-ttu-id="7a324-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-178">The developer of the app.</span></span> <span data-ttu-id="7a324-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-180">notes</span><span class="sxs-lookup"><span data-stu-id="7a324-180">notes</span></span>|<span data-ttu-id="7a324-181">String</span><span class="sxs-lookup"><span data-stu-id="7a324-181">String</span></span>|<span data-ttu-id="7a324-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="7a324-182">Notes for the app.</span></span> <span data-ttu-id="7a324-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7a324-184">uploadState</span></span>|<span data-ttu-id="7a324-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7a324-185">Int32</span></span>|<span data-ttu-id="7a324-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="7a324-186">The upload state.</span></span> <span data-ttu-id="7a324-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7a324-188">publishingState</span></span>|[<span data-ttu-id="7a324-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7a324-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7a324-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-190">The publishing state for the app.</span></span> <span data-ttu-id="7a324-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7a324-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7a324-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7a324-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7a324-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7a324-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7a324-194">isAssigned</span></span>|<span data-ttu-id="7a324-195">Логический</span><span class="sxs-lookup"><span data-stu-id="7a324-195">Boolean</span></span>|<span data-ttu-id="7a324-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="7a324-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7a324-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a324-198">roleScopeTagIds</span></span>|<span data-ttu-id="7a324-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7a324-199">String collection</span></span>|<span data-ttu-id="7a324-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7a324-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7a324-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7a324-202">committedContentVersion</span></span>|<span data-ttu-id="7a324-203">String</span><span class="sxs-lookup"><span data-stu-id="7a324-203">String</span></span>|<span data-ttu-id="7a324-204">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="7a324-204">The internal committed content version.</span></span> <span data-ttu-id="7a324-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7a324-206">fileName</span><span class="sxs-lookup"><span data-stu-id="7a324-206">fileName</span></span>|<span data-ttu-id="7a324-207">String</span><span class="sxs-lookup"><span data-stu-id="7a324-207">String</span></span>|<span data-ttu-id="7a324-208">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-208">The name of the main Lob application file.</span></span> <span data-ttu-id="7a324-209">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7a324-210">size</span><span class="sxs-lookup"><span data-stu-id="7a324-210">size</span></span>|<span data-ttu-id="7a324-211">Int64</span><span class="sxs-lookup"><span data-stu-id="7a324-211">Int64</span></span>|<span data-ttu-id="7a324-212">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="7a324-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="7a324-213">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7a324-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7a324-214">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="7a324-214">installCommandLine</span></span>|<span data-ttu-id="7a324-215">String</span><span class="sxs-lookup"><span data-stu-id="7a324-215">String</span></span>|<span data-ttu-id="7a324-216">Командной строки для установки этого приложения</span><span class="sxs-lookup"><span data-stu-id="7a324-216">The command line to install this app</span></span>|
|<span data-ttu-id="7a324-217">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="7a324-217">uninstallCommandLine</span></span>|<span data-ttu-id="7a324-218">String</span><span class="sxs-lookup"><span data-stu-id="7a324-218">String</span></span>|<span data-ttu-id="7a324-219">В командной строке команду Удалить это приложение</span><span class="sxs-lookup"><span data-stu-id="7a324-219">The command line to uninstall this app</span></span>|
|<span data-ttu-id="7a324-220">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7a324-220">applicableArchitectures</span></span>|[<span data-ttu-id="7a324-221">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7a324-221">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7a324-222">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="7a324-222">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7a324-223">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7a324-223">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7a324-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7a324-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7a324-225">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7a324-225">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7a324-226">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7a324-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7a324-227">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="7a324-227">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="7a324-228">Int32</span><span class="sxs-lookup"><span data-stu-id="7a324-228">Int32</span></span>|<span data-ttu-id="7a324-229">Значение для минимального свободного дискового пространства, которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-229">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="7a324-230">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="7a324-230">minimumMemoryInMB</span></span>|<span data-ttu-id="7a324-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7a324-231">Int32</span></span>|<span data-ttu-id="7a324-232">Значение для минимального физической памяти, которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-232">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="7a324-233">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="7a324-233">minimumNumberOfProcessors</span></span>|<span data-ttu-id="7a324-234">Int32</span><span class="sxs-lookup"><span data-stu-id="7a324-234">Int32</span></span>|<span data-ttu-id="7a324-235">Значение для минимальное число процессоров которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-235">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="7a324-236">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="7a324-236">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="7a324-237">Int32</span><span class="sxs-lookup"><span data-stu-id="7a324-237">Int32</span></span>|<span data-ttu-id="7a324-238">Значение для минимальная скорость ЦП, которая требуется для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-238">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="7a324-239">detectionRules</span><span class="sxs-lookup"><span data-stu-id="7a324-239">detectionRules</span></span>|<span data-ttu-id="7a324-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7a324-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="7a324-241">Определение правил для обнаружения Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-241">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7a324-242">installExperience</span><span class="sxs-lookup"><span data-stu-id="7a324-242">installExperience</span></span>|[<span data-ttu-id="7a324-243">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="7a324-243">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="7a324-244">Опыт установки для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7a324-244">The install experience for this app.</span></span>|
|<span data-ttu-id="7a324-245">returnCodes</span><span class="sxs-lookup"><span data-stu-id="7a324-245">returnCodes</span></span>|<span data-ttu-id="7a324-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7a324-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="7a324-247">Коды возврата для записи поведение при установке.</span><span class="sxs-lookup"><span data-stu-id="7a324-247">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="7a324-248">msiInformation</span><span class="sxs-lookup"><span data-stu-id="7a324-248">msiInformation</span></span>|[<span data-ttu-id="7a324-249">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="7a324-249">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="7a324-250">Подробности MSI, если это приложение Win32 представляет собой приложение MSI.</span><span class="sxs-lookup"><span data-stu-id="7a324-250">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="7a324-251">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="7a324-251">setupFilePath</span></span>|<span data-ttu-id="7a324-252">String</span><span class="sxs-lookup"><span data-stu-id="7a324-252">String</span></span>|<span data-ttu-id="7a324-253">Относительный путь к файлу программы установки в пакете зашифрованные Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="7a324-253">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="7a324-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a324-254">Response</span></span>
<span data-ttu-id="7a324-255">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a324-255">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a324-256">Пример</span><span class="sxs-lookup"><span data-stu-id="7a324-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a324-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a324-257">Request</span></span>
<span data-ttu-id="7a324-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a324-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2285

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="7a324-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a324-259">Response</span></span>
<span data-ttu-id="7a324-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7a324-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2457

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```




