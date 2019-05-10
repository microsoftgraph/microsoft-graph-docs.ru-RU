---
title: Наборы данных, регионы и приемники, поддерживаемые подключением к данным Microsoft Graph
description: Описаны поддерживаемые наборы данных и типы конечных хранилищ, которые можно использовать с подключением к данным Microsoft Graph.
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: fee7daae0af6ee4a1dc3d887e09acd725a37ceb8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629847"
---
# <a name="datasets-regions-and-sinks-that-microsoft-graph-data-connect-supports"></a>Наборы данных, регионы и приемники, поддерживаемые подключением к данным Microsoft Graph

Подключение к данным Microsoft Graph поддерживает разные наборы данных, регионы данных и места хранения в Microsoft Azure. В этой статье описаны поддерживаемые наборы данных и способы доступа к схемам наборов данных, поддерживаемые регионы Office 365 и Microsoft Azure, а также места хранения, используемые подключением к данным с помощью фабрики данных Azure.

Чтобы запросить поддержку дополнительных наборов данных, регионов или приемников, свяжитесь с нами в [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581).

## <a name="datasets"></a>Наборы данных

В настоящий момент подключение к данным поддерживает следующие наборы данных. Чтобы просмотреть схемы для каждого набора данных, создайте новый набор данных в фабрике данных Azure и используйте для просмотра вкладку "Схема". 

|Имя набора данных|Описание|
|-------------|-----------|
|BasicDataSet_v0.Contact_v0|Содержит контактные данные из адресной книги каждого пользователя. Схема для этих объектов напоминает [схему личных контактов Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/contact).| 
|BasicDataSet_v0.Event_v0|Содержит события из календаря каждого пользователя. Схема для этих объектов напоминает [схему событий календаря Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/event).| 
|BasicDataSet_v0.Message_v0|Содержит сообщение из почтового ящика каждого пользователя. Схема для этих объектов напоминает [схему сообщений Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/message).| 
|BasicDataSet_v0.SentItem_v0|Содержит сообщения, отправленные из почтового ящика каждого пользователя. Схема для этих объектов напоминает [схему сообщений Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/message).| 
|BasicDataSet_v0.User_v0|Содержит сведения о пользователе (DisplayName, UserPrincipalName и т. д.).| 
|BasicDataSet_v0.MailboxSettings_v0|Содержит параметры почтового ящика каждого пользователя. Схема для этих объектов соответствует [схеме параметров почтового ящика Microsoft Graph](https://docs.microsoft.com/en-us/graph/api/resources/mailboxsettings?view=graph-rest-1.0).| 
|BasicDataSet_v0.MailFolder_v0|Содержит папки почты из почтового ящика каждого пользователя. Схема для этих объектов соответствует [схеме папок почты Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/mailfolder).|
|BasicDataSet_v0.Manager_v0|Содержит сведения о пользователе для руководителя каждого пользователя. Схема для этих объектов соответствует [схеме пользователей Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user).|
|BasicDataSet_v0.DirectReport_v0|Содержит сведения о сотрудниках, находящихся в непосредственном подчинении каждого пользователя. Схема для этих объектов соответствует [схеме пользователей Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user).|
|BasicDataSet_v0.CalendarView_v0|Содержит события. Схема для этих объектов соответствует [схеме пользователей Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/events).|
|BasicDataSet_v0.User_v1|Эта таблица содержит сведения о пользователе. Схема для этих объектов соответствует [схеме пользователей Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/user).|
|BasicDataSet_v0.Contact_v1|Содержит контактные данные из адресной книги каждого пользователя. Схема для этих объектов соответствует [схеме личных контактов Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/contact).|
|BasicDataSet_v0.Event_v1|Содержит события из календаря каждого пользователя. Схема для этих объектов соответствует [схеме событий календаря Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/event).|
|BasicDataSet_v0.Message_v1|Содержит сообщение из почтового ящика каждого пользователя. Схема для этих объектов соответствует [схеме сообщений Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/message).|
|BasicDataSet_v0.SentItem_v1|Содержит сообщение, отправленное из почтового ящика каждого пользователя. Схема для этих объектов соответствует [схеме сообщений Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/message).|

## <a name="regions"></a>Регионы

Подключение к данным поддерживает извлечение данных из множества разных регионов Office 365. Чтобы успешно перенести данные из центра обработки данных Office 365 в свое хранилище Microsoft Azure, экземпляр фабрики данных Azure и место хранения Azure должны быть сопоставлены с поддерживаемым регионом для расположения данных Office 365. В следующей таблице указаны поддерживаемые регионы Office 365 и соответствующие регионы Azure, необходимые для перемещения данных. 

| Регион Office                    | Регион Azure                                |
|----------------------------------|---------------------------------------------|
| **Северная Америка**                | Восток США<br/>Восток США 2<br/>Центр США<br/>Центральный север США<br/>Центральный юг США<br/>Центральный запад США<br/>Запад США<br/>Запад США 2|
| **Европа**                       | Северная Европа<br/>Западная Европа|
| **Азиатско-Тихоокеанский регион**                 | Восточная Азия<br/>Юго-Восточная Азия|
| **Австралия**                    | Восток Австралии<br/>Юго-восток Австралии|

## <a name="sinks"></a>Приемники

Приемники — это выходное расположение, используемое фабрикой данных для размещения данных в хранилище Azure. Подключение к данным поддерживает следующие типы приемных хранилищ:

- Azure Data Lake Storage 2-го поколения
- Хранилище BLOB-объектов Azure
- Azure Data Lake Storage 1-го поколения

К приемникам применяются следующие характеристики: 

- Формат выходных файлов: строки JSON. Выходной формат является фиксированным, и его изменение не поддерживается. Однако вы можете использовать фабрику данных Azure для копирования результата конвейера подключения к данным в другой механизм хранения (например, в базу данных Azure SQL).
- Проверка подлинности субъекта-службы является единственным поддерживаемым механизмом проверки подлинности для всех типов приемников при выполнении копирования с использованием Office 365 в качестве источника.
- При использовании хранилища BLOB-объектов Azure в качестве приемника нужно убедиться, что у вашего приложения есть доступ участника данных хранилища BLOB-объектов к расположению хранилища BLOB-объектов Azure.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения о создании конвейеров подключения к данным в рамках фабрики данных Azure см. в [документации по соединителю Office 365 фабрики данных Azure](https://docs.microsoft.com/ru-RU/azure/data-factory/connector-office-365).  
