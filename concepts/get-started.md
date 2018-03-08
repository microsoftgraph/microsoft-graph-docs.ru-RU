# <a name="getting-started-building-microsoft-graph-apps"></a>Начало создания приложений Microsoft Graph

Статьи, перечисленные в этом разделе, содержат подробные указания по созданию приложений для подключения к Microsoft Graph на различных языках и платформах разработки. В каждой статье используется начальный проект и описываются основные действия для подключения к Microsoft Graph:

 1. Регистрация приложения
 2. Проверка подлинности пользователя и получение маркера доступа в приложении
 3. Вызов Microsoft Graph из приложения
 4. Запуск приложения

Чтобы быстрее получить работоспособное решение, попробуйте наше [средство быстрого создания](https://developer.microsoft.com/graph/quick-start).

Каждый готовый проект идентичен [примеру подключения в репозитории Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) для соответствующей платформы.

Хотите увидеть еще больше кода?

Ознакомьтесь с [примерами Microsoft Graph](https://github.com/microsoftgraph) на сайте GitHub. В приведенной ниже таблице перечислены дополнительные версии примеров, рассматриваемых в этом разделе. В них показано, как выполнить аутентификацию пользователя с помощью обеих конечных точек ADAL (версий 1.0 и 2.0), и используются либо необработанные вызовы REST, либо клиентская библиотека Microsoft Graph (SDK) для подключения к Microsoft Graph.

Выберите статью, посвященную вашему поставщику проверки подлинности и платформе разработки, и приступайте к подключению к Microsoft Graph. Дополнительные сведения см. в статье [Чем отличается конечная точка версии 2.0?](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/active-directory-v2-compare)


|Платформа |Конечная точка Azure AD |Конечная точка Azure AD версии 2.0 |
|:--- |:--- |:---|
|Android |<a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">Пример с использованием пакета SDK</a> |<a href="https://github.com/microsoftgraph/android-java-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST</a> |
|AngularJS |<a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/angular-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST</a> |
|ASP.NET |<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/aspnet-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST</a> |
|iOS (Obj-C) |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">Пример с использованием пакета SDK</a> |
|iOS (Swift) |<a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/ios-swift-connect-sample">Пример с использованием пакета SDK</a> |
|NodeJS |<a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/nodejs-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST</a> |
|PHP |<a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/php-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST</a> |
|Python |<a href="https://github.com/microsoftgraph/python-sample-auth/blob/master/sample_adal.py">Пример с использованием REST</a> |<a href="https://aka.ms/graph-python-samples">Пример с использованием REST</a>
|Ruby |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">Пример с использованием REST</a> |
|UWP |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">Пример с использованием REST</a> |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">Пример с использованием пакета SDK</a> или <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST</a> |
|Xamarin | |<a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">Пример с использованием пакета SDK</a> |

<br/>

## <a name="see-also"></a>См. также

- [Опробуйте примеры вызовов REST в песочнице Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer)
- [Документация по конечной точке Azure AD](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/active-directory-developers-guide)
- [Документация по конечной точке Azure AD версии 2.0](https://docs.microsoft.com/ru-RU/azure/active-directory/develop/active-directory-appmodel-v2-overview)
