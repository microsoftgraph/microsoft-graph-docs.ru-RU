---
title: Обзор подключения к данным Microsoft Graph
description: Подключение к данным Microsoft Graph предоставляет данные Microsoft 365 в Microsoft Azure, что обеспечивает доступ к наилучшим средствам разработки и размещения для работы с этими данными.
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9f93d895213c37858cf19db2b36c1f467e92fda5
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897304"
---
# <a name="overview-of-microsoft-graph-data-connect"></a>Обзор подключения к данным Microsoft Graph
Microsoft Graph содержит разнообразные данные о сотрудниках и их рабочих местах, включая сведения о том, как люди работают, общаются, выполняют совместные задания и управляют своим временем. Подключение к данным Microsoft Graph предоставляет набор инструментов для упрощения доставки данных в Microsoft Azure, что обеспечивает доступ к наилучшим средствам разработки и размещения для работы с этими данными. Это позволяет клиентам использовать преимущества инновационных или отраслевых приложений, которые повышают производительность и обеспечивают полный контроль над данными Microsoft Graph. Корпорация Майкрософт также предлагает более безопасные средства управления, ожидаемые клиентами.

## <a name="why-use-microsoft-graph-data-connect"></a>Зачем использовать подключение к данным Microsoft Graph?
Администраторы Microsoft 365 должны тщательно изучить трудности, связанные с перемещением существенных объемов данных организации и управлением ими. Подключение к данным Microsoft Graph предназначено для предоставления администраторам новых элементов управления данными. Эти данные можно использовать для создания приложений, выполняющих анализ на основе данных. 

### <a name="enable-granular-consent"></a>Включение фрагментарного согласия

В модели согласия Microsoft Graph администратор или пользователь может только разрешить или отклонить запрос приложения на доступ к конкретному, заранее определенному набору объектов. Например, запрос для Mail.Read содержит доступ для чтения к фиксированному набору объектов, поддерживающих почту Outlook, включая все экземпляры объекта [message](/graph/api/resources/message?view=graph-rest-1.0) со всеми его свойствами. С другой стороны, подключение к данным Microsoft Graph поддерживает более фрагментированное согласие, позволяя приложениям запрашивать доступ к определенным свойствам объекта или фильтровать данные в этих свойствах. Перед предоставлением доступа администраторы должны предоставить явное разрешение на доступ к данным Microsoft Graph. В запросе должен быть указан нужный уровень доступа и описано применение политики данных, причина запроса и схема запрошенных данных. В результате приложения смогут использовать только данные, важные для их работы, с исключением несвязанного содержимого. Например, приложение может использовать метаданные сообщений электронной почты, но исключать основное содержимое и вложения. 

### <a name="provide-data-governance"></a>Обеспечение управления данными
Корпорация Майкрософт поддерживает тесное разностороннее взаимодействие между Microsoft Graph и Azure с учетом состояния данных клиентов. При создании приложения с помощью подключения к данным Microsoft Graph можно указать набор подробных политик, которые предполагается соблюдать. После этого администраторы Microsoft 365 смогут просмотреть и разрешить эти политики. Такой подход снижает затраты на управление соответствием требованиям. При предоставлении разрешения корпорация Майкрософт следит за соблюдением политики приложением. Если приложение нарушает (или пытается нарушить) политику, установленную в организации, корпорация Майкрософт останавливает поток данных к этому приложению. 

### <a name="get-access-to-data-at-scale"></a>Получение доступа к данным в масштабе
Многофункциональные приложения требуют доступа к большим объемам данных, часто от многих пользователей организации одновременно. При использовании обычной транзакционной модели необходимо создать сложную инфраструктуру и выполнять тысячи вызовов API, чтобы управлять предоставлением этих данных. Подключение к данным Microsoft Graph использует возможности фабрики данных Azure для предоставления приложению данных Microsoft 365 из вашей организации с использованием повторяющегося расписания с помощью лишь нескольких простых действий.

## <a name="next-steps"></a>Дальнейшие действия
Чтобы приступить к работе, ознакомьтесь со статьей [Начало работы с подключением к данным Microsoft Graph](data-connect-get-started.md).
